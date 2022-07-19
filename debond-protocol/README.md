# D/bond Protocol: 

This Repo explains the core modules of the D/bond Protocol for developers.

On higher level, Debond protocol provides the setup for issuance of  EIP-3475 compliant  bonds along with the corresponding decentralized exchange handling the liquidity, custodian of the asset and bond price logic and secondary market.

## Overall architecture:
## [Diagram in Miro](https://miro.com/app/board/uXjVOQsK09c=/?moveToWidget=3458764519928245265&cot=14):

## 1.[Debond-Airdrop]():
    - For allowing Debond tokens to be claimed by the users which is allocated by user

## 2.[Debond-APM](https://github.com/Debond-Protocol/Debond-APM/tree/Documentation):
    - This consist of Automated Pair Maker contract that manages the liquidity via  managing  single token whenever the bonds are issued/redeemed.
    - Its called via [APMRouter](https://github.com/Debond-Protocol/Debond-Bank/blob/main/contracts/APMRouter.sol) contract for adding / removal of the liquidity along with swapping with the ERC20 collateral.

## 3.[Debond-Bank]():
    - This is the custodian of the issuance of the bonds and liquidity management. 
    - Also allows the management of the bonds.
## 4. [Debond-ERC3475](): 
    -  this are the debond version of EIP-3475 standard for generating bonds and associated functionality. always called by the bonds 