## Debond-Bank:

This repository consist of the contracts  that manage the issuance and  redemption of bonds and interfacing with the APM to permit addition/subtraction of the liquidity respectively, thus being the core part of protocol that  interfaces with Bonds contract.


## Contracts: 
1.  Bank Contract :   This contract acts as custodian of bonds by allowing buy/stake bonds with their collaterals being  ERC20 (DBIT/DGOV or other whitelisted tokens)/WETH . Only the class of bonds that are agreed upon by the governance can be issued by the functions of the contract.  Bonds are instantiated into different class  based upon the underlying collateral, nature of issuance/ redemption condition (fixed/floating rate bonds). 


2. BankBondManager: abstract contract inherited by Bank contract  for interacting directly with the  DebondBond contract to issue bonds, creating nonce , finding the bondProgress towards maturity, etc. 

3. BankData: Storage contract with  bank structures defined below: 
```solidity

    mapping(uint256 => mapping(uint256 => bool)) _canPurchase; // mapping(class(BondERC20) => class(DebondTokenBond) => bool isPurchasable).

    // other structures for finding the average liquidity and other parameters. 

    //classIdsPerTokenAddress(ERC20 => associated classIds)....etc
```

## Workflow:

    1. First User / external contract selects the type of bond that is to be purchased by two types:
        - Staking bonds allows users to earn principal interest in the form of DBIT at the time of issuance of the bonds.   user puts some amount of  WETH/ERC20 collateral to get similar amount of ERC20-Bonds and  some part of  DBIT
            - DBIT  that need to be minted is determined by the ([CDP formula value in USD]() * rateOfInterest).
            - and the given collateral is added into APM via APMRouter.

        based on whether the staking collateral is Debond Token  and corresponding input collateral is WETH or other whitelisted tokens in pairs, you have the inferface of functions as follows: 
    
        ```solidity
    function stakeForDbitBondWithEth(
        uint _WETHClassId, 
        uint _debondClassId, 
        uint _minRate,
        uint deadline,
        address _to
    ) external payable ensure(deadline);

    function stakeForDgovBondWithEth(
        uint _WETHClassId, 
        uint _debondClassId,
       uint _minRate,
        uint deadline,
        address _to
    ) external payable ensure(deadline);
    
        ```
        - Buying bonds allows issuance of bonds in pair of ERC20 with either DBIT/DGOV. when user deposits the collateral of some amount , he gets equal amount of both type of bonds .  


    2. Now user can track the progress of the bonds. based on the nature of the bond redemption condition, the frontend can use the function:

        ```solidity
        function getETA(uint256 classId, uint256 nonceId) external view returns (uint256);
        ```
    which will give time in  seconds when the bond (both fixed rate / floating rate) can be redeemed. 
        ```

**NOTE:** for fixed rate its consistent whereas for floating rate it will be an approximation and will really depend on the current availablity of liquidity for bonds using the formula ```

## Security Considerations: 

- Insure that bank contract has addresses for governance and APM correctly set else it might cause loss of the  underlying liquidity as bonds. 

### running the test.

```bash
> npm install  

> npx truffle compile


> npm run generate-types # for tests in typescript.

## and  finally running tyhe command in parallel.

> npx run ganache -p 7545 
&&
> npx truffle run test

```
### Deployment test: 

1. Add the deployment address key in .env with the RPC .

2. deployment of the contract on the given chain:

```bash
> truffle compile 

> truffle deploy 
```

3. And then trigger the function `setBankAddress()` from    which will be initializing the bank contracts across other contracts in the Debond contracts. 


## inheritance diagram: 


[bank contracts dependencies general diagram](./docs/BankContracts.png).

[Bank functions overview](./docs/BankFunctions.svg).

## Deployed contracts: 


Verifying Bank
Pass - Verified: https://rinkeby.etherscan.io/address/0xd9F6aEbEd44ea0071c1929b2bf5a3Dd671c39006#code

Verifying APMTest
Already Verified: https://rinkeby.etherscan.io/address/0xA361763C11cf4D55bD0356b4921D781BEa558325#code

Verifying DebondMath
Pass - Verified: https://rinkeby.etherscan.io/address/0xcEC56a9d7c618A0D710d362e123B979716F427fA#code
