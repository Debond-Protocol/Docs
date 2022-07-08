## Debond Governance:

Contracts that handle the upgradation of the protocol parameters and capital allocation  by allowing the DGOV holders to participate in the process either via adding the proposal to be considered for voting or voting itself for the already existing proposal. the contracts  definition are inspired  from  the modified version of[openzeppelin governance](https://github.com/OpenZeppelin/openzeppelin-contracts/tree/master/contracts/governance).  

There are two main  types of contracts present in the  debond governance:
    - Core governance contract : it consist of the main governance contract, GovernanceSharedStorage and Executable contract that holds the logic for the lifecycle of proposals for debond protocol (explained further in contracts section). 
    
    - Vote token/staking contract: these contracts provide mechanism for DGOV holders to stake  their tokens into Vote tokens (for voting purpose as well as getting interest on their staking).


## Structures: 

- the proposals are divided into several classes, each class stores information about the proposal lifecycle: 
    - timelock: Is the time period after issuance proposal, during which vote are to be locked. 
    - minimum_approval_percentage_needed: Is the minimum quorum needed to approve the proposal.
    - Architect approval: bool for checking whether the given proposal is to be approved by the Architect(ie the Veto address). 
    - maximum execution time: Is the max time after the finishing of the voting period for approved proposal, before which the proposal should be executed. 
    
    ```solidity
        mapping(uint128 => uint256[6]) public proposalClassInfo;
        // with the mapping starting from  proposalClassInfo[_proposalClass][0] = timelock, proposalClassInfo[_proposalClass][0] = min_approval_percent and so on .... 
    ```
    -  proposal class 1 and 2 have the proposals with highest priority to be checked by the veto address (ie multisig address being the deployer of all the contract) and it has  higher timelock and approval percentage needed. 

- each proposal stores the following information: 
    ```solidity
 struct  Proposal {
        uint256 startTime;
        uint256 endTime;
        address proposer;
        ProposalStatus status;
        ProposalApproval approvalMode;
        address[] targets;
        uint256[] values;
        bytes[] calldatas;
        bytes32 descriptionHash;
    }
    ```
    where most of the information is self explanatory, and ProposalStatus is an enum that represents the state of the proposal (Active,Canceled,Pending,Defeated,Succeeded,Executed) and ProposalApproval enum determines the nature of the evaluation of the proposal. this is defined by the following conditions: 
        1. NoVote : for the proposal by  core address of debond 
        2. Approve: the proposal is approved the moment it gets sufficient pro votes.
        3. ApproveAndVeto: the veto condition (explained in **Working process**)

    - targets is the address array of the contract proposal that has been passed and will then be called by the given entity.

    - values are the parameters of the functions that are to be executed based on the proposal.

    - 


## Contracts:

### storages: 

1. [VoteStorage](): This stores the structures and mappings referred by  vote token for referring to the votes calculation process (explained in voteCounting contract).

2. [NewGovStorage](): This contract stores the mapping of the proposals issued by the governance participants 

//TODO: merge this into one or rename 
### utils: 
1. [GovSettings](): Contract that defines the function for setting the delay of starting voting period after proposal creation. 

2. [VoteCounting](): This stores the function for storing the votes by participant for proposal, along with function to find the sufficient quorum for the functions.
## Contract.

**1. Core contracts**

1. [NewGovernance](): Core contract with the functions to issue the setup of the proposal,  proposal and vote cr creation, cancellation  etc. internally it interacts with the storage , staking and vote token to provide the main functionalities for governance along with the different projects.
2. [StakingDGOV](): manages the staking process of the DGOV token in order to generate the Vote Token along with accumulated interest when the voting period is completed.

3. [Vote](): ERC20 token issued for the participation the the voting process, when user stakes their DGOV token. they are not P2P transferrable (only within the voting process). 



**2.Storage contracts**

1. [GovStorage and govShared Storage](): These contracts store the  mapping information about the proposal details, voting parameters , token allocation etc.

2. [VoteStorage](): consist of  mappings and structs that  stores the available vote tokens, accumulated interest in DBIT (based on number of the days voting participation, etc).


## Working process:

1. Proposal creator (with DGOV tokens) adds all the values for his proposal in the frontend .
    - Proposal contract it inherits only the functions by inheriting from the interface of the governance contract. Example of the contract :[here](./contracts/Proposal/Proposal.sol). Then the Proposal time period starts and then voting starts after the delay period (defined in govSettings by the deployer/ governance) and rests till the `endTime`. 

    ```solidity
    function createProposal(
        uint128 _class,
        address[] memory _targets,
        uint256[] memory _values,
        bytes[] memory _calldatas,
        string memory _description
    )
    ```

2. On the voter side, they stake their tokens in the StakingDGOV contract, which then mints equivalent number of vote tokens for him and puts his DGOV tokens on timelock. Voters are also incentivised by providing them intererst in DBIT once the timelock passes, and their interest depends upon the number of days the user has voted on any proposal. 

3. Once the proposal endtime passes, the frontend checks for the proposal votes (pro,con) and if it satisfies both conditions (pro > con along with the votes being greater than minimum approval votes in the given proposal class). 
    - then we check if veto is required (specially for proposal nonces in class 1 or 2), if yes then veto address will finally determine the fate of proposal status (Accepted/ rejected).
    - else the accepted proposal can be executed by the proposer

4. And then eventually voters can redeem their unused VOTE token back to DGOV, and recovering the DBIT interest.  

## Security Considerations:

- insure that governance veto address (debondOperator) should be secured by multisig as it has override on some parameters and proposals having `noVote` conditions.
- also there is no standardised interface of proposals, thus for the proposals being introduced by the external community members (unless verified) needs to have more scrutiny about the implementation (like having verified contracts and having delay in the proposal execution after voting, etc).

## usage: 

1. For the deployment
    - Add .env private key for the deployment (and defining the `debondOperator`).
    - define the [HDWallet](https://www.npmjs.com/package/@truffle/hdwallet-provider) in the core repo.
    - then run
    ```bash
     $ truffle deploy --network .
    - then define the address of the governance contracts in each of the other contracts (from utils/governanceOwnable.sol).

    ```
2. for importing the smart contracts package:
    ```solidity
    // for defining the proposal smart contract.
    import "debond-governance/contracts/INewExecutable.sol";
    import "debond-governance/contracts/utils/IGovernanceOwnable.sol";
    import "debond-governance/contracts/interfaces/INewGovernance.sol";
    contract testProposal {
    //... see example implementation in Proposal/Proposal.sol.
    
    }
    }

    }
    
```



## Contracts dependence diagram:
### 1. inheritance diagram: 

![](./contracts/docs/governance_inheritance_diagram.png)


###  2. NewGovernance function call diagram: 

![](./contracts/docs/governance_graph.png)


