

As explained in the  whitepaper, the debond protocol  consists of two types of tokens
DBIT: 
This represents an un-capped supply token that acts as the utility token for the protocol. all the interest from the primary  and secondary markets will be transferred via the given results and thus here we can get better 
DBIT token has 3 types of supply :
Collateralized Supply: This total supply is equal to the CDP quantity of the bonds issued (either via the staking/buying process). the price is defined by the following formula: 
                                    
Where  S(total) is the minted bonds during the issuance process. 
Allocated Supply: This is the total supply corresponding to all addresses that are contributors in the d/bond-protocol (as core team developers and community participants recognized by the governance ) and has tokens that can be minted by the team members only after passing the proposal. Also, we will be using mechanisms like vesting in order to ensure the transparency of tokenomics. for more about the functions used, check debond-governance.
Airdropped Supply: This total supply is reserved for the community members whose addresses are allocated the tokens. based on the given time period, the user can mint this token which will then be added to the Airdropped Supply. 
Also, there is another supply (that is not separately monitored ) called as lockedSupply that is checked for a given address in order to determine how many of the given collateralized supply are being locked at the same time as the creation of the bonds (and thus are "virtually locked" in the liquidity pool).
the formula is  defined  as follows: 
function getLockedBalance(address account)
        public
        view
        returns (uint256 _lockedBalance)
    {
         // max 5% of collateralized supply can be transferred
        uint256 _maxUnlockable = _collateralisedSupply * 5;
        // multiplying by 100, since _maxUnlockable isn't divided by 100
        uint256 _currentAirdropSupply = _airdropSupply * 100;

        _lockedBalance = 0;
        if (_currentAirdropSupply > _maxUnlockable) {
            _lockedBalance =
                ((100 - (_maxUnlockable * 100) / _currentAirdropSupply) *
                    _airdropBalance[account]) /
                100;
        }
        return _lockedBalance;
    }
2. DGOV tokens: 
 These are governance tokens for allowing holders to add proposals in the debond governance for protocol upgradation and decisions related to the treasury, as well as participating in the voting process, by staking the DGOV tokens(more information is defined in the Debond-governance). it uses all the underlying functions of the debondToken, except being limited in the maximum in the defined supply.

Contracts:
DebondToken.sol : The common implementation interface for minting and supply getter/ setter functions for DBIT/DGOV tokens. 
pragma solidity ^0.8.9;

// SPDX-License-Identifier: apache 2.0
/*
    Copyright 2022 Debond Protocol <info@debond.org>
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    http://www.apache.org/licenses/LICENSE-2.0
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
*/
interface IDebondToken {
    ///@dev returns airdroppped + allocated + unlocked collateralised supply of tokens
    function totalSupply() external view returns (uint256);
    ///@dev returns the total unlocked collateralised supply
    function getTotalCollateralisedSupply() external view returns (uint256);
    ///@dev returns the total airdroppedSupply currently being claimed already.
    function getTotalAirdropSupply() external view returns (uint256);
    /// @dev returns the max airdrop supply that can be claimed by the whitelisted users.
    function getMaxAirdropSupply() external view returns (uint256);
    /// @dev gives total allocated supply by the governance.
    function getTotalAllocatedSupply() external view returns (uint256);
    /// @dev gives max total allocation of the tokens unlocked of the total allocation. 
    function getMaxAllocatedPercentage() external view returns (uint256);
    /// @dev fetching the total balance overall of the given token (DBIT/DGOV).
    function getTotalBalance(address _of) external view returns (uint256);
    /// @dev  fetches the lockedBalance(amount of tokens being collateralised and not redeemed).
    function getLockedBalance(address account)
        external
        view
        returns (uint256 _lockedBalance);
    /// @dev transfer tokens top given destination address (given msg.sender has amount > total - getLockedBalance())
    function transfer(address _to, uint256 _amount) external returns (bool);
    /// @dev transfers the token from given addresses (_from -> _to) given that unlockedTokens are greater than _amount.
    function transferFrom(
        address _from,
        address _to,
        uint256 _amount
    ) external returns (bool);

    /// @dev : allows airdrop.claim(address _addr) to mint the airdropSupply of the given whitelisted user. 
    function mintAirdropSupply(address _to, uint256 _amount) external;
    /// @dev : allows bank and exchangfe 
    function mintCollateralisedSupply(address _to, uint256 _amount) external;

    function mintAllocatedSupply(address _to, uint256 _amount) external;

    function getCollateralisedBalance(address _of)
        external
        view
        returns (uint256);

    function getAllocatedBalance(address _of) external view returns (uint256);

    function getAirdropBalance(address _of) external view returns (uint256);

    function setMaxAirdropSupply(uint256 new_supply) external returns (bool);

    function setMaxAllocationPercentage(uint256 newPercentage)
        external
        returns (bool);

    function setBankAddress(address _bankAddress) external;

    function setAirdropAddress(address _airdropAddress) external;
    
    function setExchangeAddress(address _exchangeAddress) external;   
}
2. DGOV.sol:  it inherits most of the methods from DebondToken except for the modifiers  that check the condition of unlocking supply (i.e mintCollateralisedSupply ), transfer functions and eventually 
3. DBIT.sol: it also inherits the interface from the DebondToken with the uncapped supply.
Installation: 
$ npm install @debond/Token.

Integration Steps : 
First insure you have defined the bank address and other roles for the smart contract . this 

import "@debond/token/contracts/IDebondToken.sol";


contract demoToken is IDebondToken {
.......
}
