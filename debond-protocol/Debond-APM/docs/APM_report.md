## Sūrya's Description Report

### Files Description Table


|  File Name  |  SHA-1 Hash  |
|-------------|--------------|
| contracts/APM.sol | 77c310ddee4ae4a86af2c84f34aff197325d4ec4 |


### Contracts Description Table


|  Contract  |         Type        |       Bases      |                  |                 |
|:----------:|:-------------------:|:----------------:|:----------------:|:---------------:|
|     └      |  **Function Name**  |  **Visibility**  |  **Mutability**  |  **Modifiers**  |
||||||
| **APM** | Implementation | IAPM, GovernanceOwnable |||
| └ | <Constructor> | Public ❗️ | 🛑  | GovernanceOwnable |
| └ | setBankAddress | External ❗️ | 🛑  | onlyGovernance |
| └ | getReservesOneToken | Private 🔐 |   | |
| └ | getReserves | Public ❗️ |   |NO❗️ |
| └ | updateTotalReserve | Public ❗️ | 🛑  |NO❗️ |
| └ | getVlps | Public ❗️ |   |NO❗️ |
| └ | updateWhenAddLiquidityOneToken | Private 🔐 | 🛑  | |
| └ | updateWhenAddLiquidity | External ❗️ | 🛑  | onlyBank |
| └ | updateWhenRemoveLiquidityOneToken | Private 🔐 | 🛑  | |
| └ | updateWhenRemoveLiquidity | Public ❗️ | 🛑  |NO❗️ |
| └ | updateWhenSwap | Private 🔐 | 🛑  | |
| └ | amountToAddVlp | Public ❗️ |   |NO❗️ |
| └ | amountToRemoveVlp | Public ❗️ |   |NO❗️ |
| └ | swap | External ❗️ | 🛑  |NO❗️ |
| └ | getAmountOut | Internal 🔒 |   | |
| └ | getAmountsOut | External ❗️ |   |NO❗️ |
| └ | removeLiquidity | External ❗️ | 🛑  | onlyBank |


### Legend

|  Symbol  |  Meaning  |
|:--------:|-----------|
|    🛑    | Function can modify state |
|    💵    | Function is payable |
