├─ type: SourceUnit
└─ children
   ├─ 0
   │  ├─ type: PragmaDirective
   │  ├─ name: solidity
   │  └─ value: ^0.8.0
   ├─ 1
   │  ├─ type: ImportDirective
   │  ├─ path: ./interfaces/IAPM.sol
   │  ├─ unitAlias
   │  └─ symbolAliases
   ├─ 2
   │  ├─ type: ImportDirective
   │  ├─ path: @openzeppelin/contracts/token/ERC20/IERC20.sol
   │  ├─ unitAlias
   │  └─ symbolAliases
   ├─ 3
   │  ├─ type: ImportDirective
   │  ├─ path: @openzeppelin/contracts/token/ERC20/utils/SafeERC20.sol
   │  ├─ unitAlias
   │  └─ symbolAliases
   ├─ 4
   │  ├─ type: ImportDirective
   │  ├─ path: debond-governance-contracts/utils/GovernanceOwnable.sol
   │  ├─ unitAlias
   │  └─ symbolAliases
   └─ 5
      ├─ type: ContractDefinition
      ├─ name: APM
      ├─ baseContracts
      │  ├─ 0
      │  │  ├─ type: InheritanceSpecifier
      │  │  ├─ baseName
      │  │  │  ├─ type: UserDefinedTypeName
      │  │  │  └─ namePath: IAPM
      │  │  └─ arguments
      │  └─ 1
      │     ├─ type: InheritanceSpecifier
      │     ├─ baseName
      │     │  ├─ type: UserDefinedTypeName
      │     │  └─ namePath: GovernanceOwnable
      │     └─ arguments
      ├─ subNodes
      │  ├─ 0
      │  │  ├─ type: UsingForDeclaration
      │  │  ├─ typeName
      │  │  │  ├─ type: UserDefinedTypeName
      │  │  │  └─ namePath: IERC20
      │  │  └─ libraryName: SafeERC20
      │  ├─ 1
      │  │  ├─ type: StateVariableDeclaration
      │  │  ├─ variables
      │  │  │  └─ 0
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: Mapping
      │  │  │     │  ├─ keyType
      │  │  │     │  │  ├─ type: ElementaryTypeName
      │  │  │     │  │  └─ name: address
      │  │  │     │  └─ valueType
      │  │  │     │     ├─ type: ElementaryTypeName
      │  │  │     │     └─ name: uint256
      │  │  │     ├─ name: totalReserve
      │  │  │     ├─ expression
      │  │  │     ├─ visibility: internal
      │  │  │     ├─ isStateVar: true
      │  │  │     ├─ isDeclaredConst: false
      │  │  │     ├─ isIndexed: false
      │  │  │     ├─ isImmutable: false
      │  │  │     └─ override
      │  │  └─ initialValue
      │  ├─ 2
      │  │  ├─ type: StateVariableDeclaration
      │  │  ├─ variables
      │  │  │  └─ 0
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: Mapping
      │  │  │     │  ├─ keyType
      │  │  │     │  │  ├─ type: ElementaryTypeName
      │  │  │     │  │  └─ name: address
      │  │  │     │  └─ valueType
      │  │  │     │     ├─ type: ElementaryTypeName
      │  │  │     │     └─ name: uint256
      │  │  │     ├─ name: totalVlp
      │  │  │     ├─ expression
      │  │  │     ├─ visibility: internal
      │  │  │     ├─ isStateVar: true
      │  │  │     ├─ isDeclaredConst: false
      │  │  │     ├─ isIndexed: false
      │  │  │     ├─ isImmutable: false
      │  │  │     └─ override
      │  │  └─ initialValue
      │  ├─ 3
      │  │  ├─ type: StateVariableDeclaration
      │  │  ├─ variables
      │  │  │  └─ 0
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: Mapping
      │  │  │     │  ├─ keyType
      │  │  │     │  │  ├─ type: ElementaryTypeName
      │  │  │     │  │  └─ name: address
      │  │  │     │  └─ valueType
      │  │  │     │     ├─ type: Mapping
      │  │  │     │     ├─ keyType
      │  │  │     │     │  ├─ type: ElementaryTypeName
      │  │  │     │     │  └─ name: address
      │  │  │     │     └─ valueType
      │  │  │     │        ├─ type: ElementaryTypeName
      │  │  │     │        └─ name: uint
      │  │  │     ├─ name: vlp
      │  │  │     ├─ expression
      │  │  │     ├─ visibility: default
      │  │  │     ├─ isStateVar: true
      │  │  │     ├─ isDeclaredConst: false
      │  │  │     ├─ isIndexed: false
      │  │  │     ├─ isImmutable: false
      │  │  │     └─ override
      │  │  └─ initialValue
      │  ├─ 4
      │  │  ├─ type: StateVariableDeclaration
      │  │  ├─ variables
      │  │  │  └─ 0
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: address
      │  │  │     ├─ name: bankAddress
      │  │  │     ├─ expression
      │  │  │     ├─ visibility: default
      │  │  │     ├─ isStateVar: true
      │  │  │     ├─ isDeclaredConst: false
      │  │  │     ├─ isIndexed: false
      │  │  │     ├─ isImmutable: false
      │  │  │     └─ override
      │  │  └─ initialValue
      │  ├─ 5
      │  │  ├─ type: StructDefinition
      │  │  ├─ name: UpdateData
      │  │  └─ members
      │  │     ├─ 0
      │  │     │  ├─ type: VariableDeclaration
      │  │     │  ├─ typeName
      │  │     │  │  ├─ type: ElementaryTypeName
      │  │     │  │  └─ name: uint
      │  │     │  ├─ name: amountA
      │  │     │  ├─ storageLocation
      │  │     │  ├─ isStateVar: false
      │  │     │  └─ isIndexed: false
      │  │     ├─ 1
      │  │     │  ├─ type: VariableDeclaration
      │  │     │  ├─ typeName
      │  │     │  │  ├─ type: ElementaryTypeName
      │  │     │  │  └─ name: uint
      │  │     │  ├─ name: amountB
      │  │     │  ├─ storageLocation
      │  │     │  ├─ isStateVar: false
      │  │     │  └─ isIndexed: false
      │  │     ├─ 2
      │  │     │  ├─ type: VariableDeclaration
      │  │     │  ├─ typeName
      │  │     │  │  ├─ type: ElementaryTypeName
      │  │     │  │  └─ name: address
      │  │     │  ├─ name: tokenA
      │  │     │  ├─ storageLocation
      │  │     │  ├─ isStateVar: false
      │  │     │  └─ isIndexed: false
      │  │     └─ 3
      │  │        ├─ type: VariableDeclaration
      │  │        ├─ typeName
      │  │        │  ├─ type: ElementaryTypeName
      │  │        │  └─ name: address
      │  │        ├─ name: tokenB
      │  │        ├─ storageLocation
      │  │        ├─ isStateVar: false
      │  │        └─ isIndexed: false
      │  ├─ 6
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name
      │  │  ├─ parameters
      │  │  │  └─ 0
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: address
      │  │  │     ├─ name: _governanceAddress
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  ├─ visibility: default
      │  │  ├─ modifiers
      │  │  │  └─ 0
      │  │  │     ├─ type: ModifierInvocation
      │  │  │     ├─ name: GovernanceOwnable
      │  │  │     └─ arguments
      │  │  │        └─ 0
      │  │  │           ├─ type: Identifier
      │  │  │           └─ name: _governanceAddress
      │  │  ├─ override
      │  │  ├─ isConstructor: true
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability
      │  ├─ 7
      │  │  ├─ type: ModifierDefinition
      │  │  ├─ name: onlyBank
      │  │  ├─ parameters
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     ├─ 0
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: require
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  ├─ operator: ==
      │  │  │     │     │  │  ├─ left
      │  │  │     │     │  │  │  ├─ type: MemberAccess
      │  │  │     │     │  │  │  ├─ expression
      │  │  │     │     │  │  │  │  ├─ type: Identifier
      │  │  │     │     │  │  │  │  └─ name: msg
      │  │  │     │     │  │  │  └─ memberName: sender
      │  │  │     │     │  │  └─ right
      │  │  │     │     │  │     ├─ type: Identifier
      │  │  │     │     │  │     └─ name: bankAddress
      │  │  │     │     │  └─ 1
      │  │  │     │     │     ├─ type: StringLiteral
      │  │  │     │     │     ├─ value: APM: Not Authorised
      │  │  │     │     │     └─ parts
      │  │  │     │     │        └─ 0: APM: Not Authorised
      │  │  │     │     └─ names
      │  │  │     └─ 1
      │  │  │        ├─ type: ExpressionStatement
      │  │  │        └─ expression
      │  │  │           ├─ type: Identifier
      │  │  │           └─ name: _
      │  │  ├─ isVirtual: false
      │  │  └─ override
      │  ├─ 8
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: setBankAddress
      │  │  ├─ parameters
      │  │  │  └─ 0
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: address
      │  │  │     ├─ name: _bankAddress
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     ├─ 0
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: require
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  ├─ operator: !=
      │  │  │     │     │  │  ├─ left
      │  │  │     │     │  │  │  ├─ type: Identifier
      │  │  │     │     │  │  │  └─ name: _bankAddress
      │  │  │     │     │  │  └─ right
      │  │  │     │     │  │     ├─ type: FunctionCall
      │  │  │     │     │  │     ├─ expression
      │  │  │     │     │  │     │  ├─ type: TypeNameExpression
      │  │  │     │     │  │     │  └─ typeName
      │  │  │     │     │  │     │     ├─ type: ElementaryTypeName
      │  │  │     │     │  │     │     └─ name: address
      │  │  │     │     │  │     ├─ arguments
      │  │  │     │     │  │     │  └─ 0
      │  │  │     │     │  │     │     ├─ type: NumberLiteral
      │  │  │     │     │  │     │     ├─ number: 0
      │  │  │     │     │  │     │     └─ subdenomination
      │  │  │     │     │  │     └─ names
      │  │  │     │     │  └─ 1
      │  │  │     │     │     ├─ type: StringLiteral
      │  │  │     │     │     ├─ value: APM: Address 0 given for Bank!
      │  │  │     │     │     └─ parts
      │  │  │     │     │        └─ 0: APM: Address 0 given for Bank!
      │  │  │     │     └─ names
      │  │  │     └─ 1
      │  │  │        ├─ type: ExpressionStatement
      │  │  │        └─ expression
      │  │  │           ├─ type: BinaryOperation
      │  │  │           ├─ operator: =
      │  │  │           ├─ left
      │  │  │           │  ├─ type: Identifier
      │  │  │           │  └─ name: bankAddress
      │  │  │           └─ right
      │  │  │              ├─ type: Identifier
      │  │  │              └─ name: _bankAddress
      │  │  ├─ visibility: external
      │  │  ├─ modifiers
      │  │  │  └─ 0
      │  │  │     ├─ type: ModifierInvocation
      │  │  │     ├─ name: onlyGovernance
      │  │  │     └─ arguments
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability
      │  ├─ 9
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: getReservesOneToken
      │  │  ├─ parameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: address
      │  │  │  │  ├─ name: tokenA
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 1
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: address
      │  │  │     ├─ name: tokenB
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  │  └─ 0
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: uint
      │  │  │     ├─ name: reserveA
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     ├─ 0
      │  │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  ├─ variables
      │  │  │     │  │  └─ 0
      │  │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     ├─ typeName
      │  │  │     │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  │     │  └─ name: uint
      │  │  │     │  │     ├─ name: totalVlpA
      │  │  │     │  │     ├─ storageLocation
      │  │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     └─ isIndexed: false
      │  │  │     │  └─ initialValue
      │  │  │     │     ├─ type: IndexAccess
      │  │  │     │     ├─ base
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: totalVlp
      │  │  │     │     └─ index
      │  │  │     │        ├─ type: Identifier
      │  │  │     │        └─ name: tokenA
      │  │  │     └─ 1
      │  │  │        ├─ type: IfStatement
      │  │  │        ├─ condition
      │  │  │        │  ├─ type: BinaryOperation
      │  │  │        │  ├─ operator: !=
      │  │  │        │  ├─ left
      │  │  │        │  │  ├─ type: Identifier
      │  │  │        │  │  └─ name: totalVlpA
      │  │  │        │  └─ right
      │  │  │        │     ├─ type: NumberLiteral
      │  │  │        │     ├─ number: 0
      │  │  │        │     └─ subdenomination
      │  │  │        ├─ trueBody
      │  │  │        │  ├─ type: Block
      │  │  │        │  └─ statements
      │  │  │        │     ├─ 0
      │  │  │        │     │  ├─ type: VariableDeclarationStatement
      │  │  │        │     │  ├─ variables
      │  │  │        │     │  │  └─ 0
      │  │  │        │     │  │     ├─ type: VariableDeclaration
      │  │  │        │     │  │     ├─ typeName
      │  │  │        │     │  │     │  ├─ type: ElementaryTypeName
      │  │  │        │     │  │     │  └─ name: uint
      │  │  │        │     │  │     ├─ name: vlpA
      │  │  │        │     │  │     ├─ storageLocation
      │  │  │        │     │  │     ├─ isStateVar: false
      │  │  │        │     │  │     └─ isIndexed: false
      │  │  │        │     │  └─ initialValue
      │  │  │        │     │     ├─ type: IndexAccess
      │  │  │        │     │     ├─ base
      │  │  │        │     │     │  ├─ type: IndexAccess
      │  │  │        │     │     │  ├─ base
      │  │  │        │     │     │  │  ├─ type: Identifier
      │  │  │        │     │     │  │  └─ name: vlp
      │  │  │        │     │     │  └─ index
      │  │  │        │     │     │     ├─ type: Identifier
      │  │  │        │     │     │     └─ name: tokenA
      │  │  │        │     │     └─ index
      │  │  │        │     │        ├─ type: Identifier
      │  │  │        │     │        └─ name: tokenB
      │  │  │        │     └─ 1
      │  │  │        │        ├─ type: ExpressionStatement
      │  │  │        │        └─ expression
      │  │  │        │           ├─ type: BinaryOperation
      │  │  │        │           ├─ operator: =
      │  │  │        │           ├─ left
      │  │  │        │           │  ├─ type: Identifier
      │  │  │        │           │  └─ name: reserveA
      │  │  │        │           └─ right
      │  │  │        │              ├─ type: BinaryOperation
      │  │  │        │              ├─ operator: /
      │  │  │        │              ├─ left
      │  │  │        │              │  ├─ type: BinaryOperation
      │  │  │        │              │  ├─ operator: *
      │  │  │        │              │  ├─ left
      │  │  │        │              │  │  ├─ type: Identifier
      │  │  │        │              │  │  └─ name: vlpA
      │  │  │        │              │  └─ right
      │  │  │        │              │     ├─ type: IndexAccess
      │  │  │        │              │     ├─ base
      │  │  │        │              │     │  ├─ type: Identifier
      │  │  │        │              │     │  └─ name: totalReserve
      │  │  │        │              │     └─ index
      │  │  │        │              │        ├─ type: Identifier
      │  │  │        │              │        └─ name: tokenA
      │  │  │        │              └─ right
      │  │  │        │                 ├─ type: Identifier
      │  │  │        │                 └─ name: totalVlpA
      │  │  │        └─ falseBody
      │  │  ├─ visibility: private
      │  │  ├─ modifiers
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability: view
      │  ├─ 10
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: getReserves
      │  │  ├─ parameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: address
      │  │  │  │  ├─ name: tokenA
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 1
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: address
      │  │  │     ├─ name: tokenB
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: reserveA
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 1
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: uint
      │  │  │     ├─ name: reserveB
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     └─ 0
      │  │  │        ├─ type: ExpressionStatement
      │  │  │        └─ expression
      │  │  │           ├─ type: BinaryOperation
      │  │  │           ├─ operator: =
      │  │  │           ├─ left
      │  │  │           │  ├─ type: TupleExpression
      │  │  │           │  ├─ components
      │  │  │           │  │  ├─ 0
      │  │  │           │  │  │  ├─ type: Identifier
      │  │  │           │  │  │  └─ name: reserveA
      │  │  │           │  │  └─ 1
      │  │  │           │  │     ├─ type: Identifier
      │  │  │           │  │     └─ name: reserveB
      │  │  │           │  └─ isArray: false
      │  │  │           └─ right
      │  │  │              ├─ type: TupleExpression
      │  │  │              ├─ components
      │  │  │              │  ├─ 0
      │  │  │              │  │  ├─ type: FunctionCall
      │  │  │              │  │  ├─ expression
      │  │  │              │  │  │  ├─ type: Identifier
      │  │  │              │  │  │  └─ name: getReservesOneToken
      │  │  │              │  │  ├─ arguments
      │  │  │              │  │  │  ├─ 0
      │  │  │              │  │  │  │  ├─ type: Identifier
      │  │  │              │  │  │  │  └─ name: tokenA
      │  │  │              │  │  │  └─ 1
      │  │  │              │  │  │     ├─ type: Identifier
      │  │  │              │  │  │     └─ name: tokenB
      │  │  │              │  │  └─ names
      │  │  │              │  └─ 1
      │  │  │              │     ├─ type: FunctionCall
      │  │  │              │     ├─ expression
      │  │  │              │     │  ├─ type: Identifier
      │  │  │              │     │  └─ name: getReservesOneToken
      │  │  │              │     ├─ arguments
      │  │  │              │     │  ├─ 0
      │  │  │              │     │  │  ├─ type: Identifier
      │  │  │              │     │  │  └─ name: tokenB
      │  │  │              │     │  └─ 1
      │  │  │              │     │     ├─ type: Identifier
      │  │  │              │     │     └─ name: tokenA
      │  │  │              │     └─ names
      │  │  │              └─ isArray: false
      │  │  ├─ visibility: public
      │  │  ├─ modifiers
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability: view
      │  ├─ 11
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: updateTotalReserve
      │  │  ├─ parameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: address
      │  │  │  │  ├─ name: tokenAddress
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 1
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: uint
      │  │  │     ├─ name: amount
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     └─ 0
      │  │  │        ├─ type: ExpressionStatement
      │  │  │        └─ expression
      │  │  │           ├─ type: BinaryOperation
      │  │  │           ├─ operator: =
      │  │  │           ├─ left
      │  │  │           │  ├─ type: IndexAccess
      │  │  │           │  ├─ base
      │  │  │           │  │  ├─ type: Identifier
      │  │  │           │  │  └─ name: totalReserve
      │  │  │           │  └─ index
      │  │  │           │     ├─ type: Identifier
      │  │  │           │     └─ name: tokenAddress
      │  │  │           └─ right
      │  │  │              ├─ type: BinaryOperation
      │  │  │              ├─ operator: +
      │  │  │              ├─ left
      │  │  │              │  ├─ type: IndexAccess
      │  │  │              │  ├─ base
      │  │  │              │  │  ├─ type: Identifier
      │  │  │              │  │  └─ name: totalReserve
      │  │  │              │  └─ index
      │  │  │              │     ├─ type: Identifier
      │  │  │              │     └─ name: tokenAddress
      │  │  │              └─ right
      │  │  │                 ├─ type: Identifier
      │  │  │                 └─ name: amount
      │  │  ├─ visibility: public
      │  │  ├─ modifiers
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability
      │  ├─ 12
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: getVlps
      │  │  ├─ parameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: address
      │  │  │  │  ├─ name: tokenA
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 1
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: address
      │  │  │     ├─ name: tokenB
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  │  └─ 0
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: uint
      │  │  │     ├─ name: vlpA
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     └─ 0
      │  │  │        ├─ type: ExpressionStatement
      │  │  │        └─ expression
      │  │  │           ├─ type: BinaryOperation
      │  │  │           ├─ operator: =
      │  │  │           ├─ left
      │  │  │           │  ├─ type: Identifier
      │  │  │           │  └─ name: vlpA
      │  │  │           └─ right
      │  │  │              ├─ type: IndexAccess
      │  │  │              ├─ base
      │  │  │              │  ├─ type: IndexAccess
      │  │  │              │  ├─ base
      │  │  │              │  │  ├─ type: Identifier
      │  │  │              │  │  └─ name: vlp
      │  │  │              │  └─ index
      │  │  │              │     ├─ type: Identifier
      │  │  │              │     └─ name: tokenA
      │  │  │              └─ index
      │  │  │                 ├─ type: Identifier
      │  │  │                 └─ name: tokenB
      │  │  ├─ visibility: public
      │  │  ├─ modifiers
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability: view
      │  ├─ 13
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: updateWhenAddLiquidityOneToken
      │  │  ├─ parameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: amountA
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  ├─ 1
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: address
      │  │  │  │  ├─ name: tokenA
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 2
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: address
      │  │  │     ├─ name: tokenB
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     ├─ 0
      │  │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  ├─ variables
      │  │  │     │  │  └─ 0
      │  │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     ├─ typeName
      │  │  │     │  │     │  ├─ type: UserDefinedTypeName
      │  │  │     │  │     │  └─ namePath: UpdateData
      │  │  │     │  │     ├─ name: updateData
      │  │  │     │  │     ├─ storageLocation: memory
      │  │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     └─ isIndexed: false
      │  │  │     │  └─ initialValue
      │  │  │     ├─ 1
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: MemberAccess
      │  │  │     │     │  ├─ expression
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: updateData
      │  │  │     │     │  └─ memberName: amountA
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: Identifier
      │  │  │     │        └─ name: amountA
      │  │  │     ├─ 2
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: MemberAccess
      │  │  │     │     │  ├─ expression
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: updateData
      │  │  │     │     │  └─ memberName: tokenA
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: Identifier
      │  │  │     │        └─ name: tokenA
      │  │  │     ├─ 3
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: MemberAccess
      │  │  │     │     │  ├─ expression
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: updateData
      │  │  │     │     │  └─ memberName: tokenB
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: Identifier
      │  │  │     │        └─ name: tokenB
      │  │  │     ├─ 4
      │  │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  ├─ variables
      │  │  │     │  │  └─ 0
      │  │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     ├─ typeName
      │  │  │     │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  │     │  └─ name: uint
      │  │  │     │  │     ├─ name: totalReserveA
      │  │  │     │  │     ├─ storageLocation
      │  │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     └─ isIndexed: false
      │  │  │     │  └─ initialValue
      │  │  │     │     ├─ type: IndexAccess
      │  │  │     │     ├─ base
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: totalReserve
      │  │  │     │     └─ index
      │  │  │     │        ├─ type: MemberAccess
      │  │  │     │        ├─ expression
      │  │  │     │        │  ├─ type: Identifier
      │  │  │     │        │  └─ name: updateData
      │  │  │     │        └─ memberName: tokenA
      │  │  │     ├─ 5
      │  │  │     │  ├─ type: IfStatement
      │  │  │     │  ├─ condition
      │  │  │     │  │  ├─ type: BinaryOperation
      │  │  │     │  │  ├─ operator: !=
      │  │  │     │  │  ├─ left
      │  │  │     │  │  │  ├─ type: Identifier
      │  │  │     │  │  │  └─ name: totalReserveA
      │  │  │     │  │  └─ right
      │  │  │     │  │     ├─ type: NumberLiteral
      │  │  │     │  │     ├─ number: 0
      │  │  │     │  │     └─ subdenomination
      │  │  │     │  ├─ trueBody
      │  │  │     │  │  ├─ type: Block
      │  │  │     │  │  └─ statements
      │  │  │     │  │     ├─ 0
      │  │  │     │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  │     │  ├─ variables
      │  │  │     │  │     │  │  └─ 0
      │  │  │     │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     │  │     ├─ typeName
      │  │  │     │  │     │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  │     │  │     │  └─ name: uint
      │  │  │     │  │     │  │     ├─ name: oldVlpA
      │  │  │     │  │     │  │     ├─ storageLocation
      │  │  │     │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     │  │     └─ isIndexed: false
      │  │  │     │  │     │  └─ initialValue
      │  │  │     │  │     │     ├─ type: IndexAccess
      │  │  │     │  │     │     ├─ base
      │  │  │     │  │     │     │  ├─ type: IndexAccess
      │  │  │     │  │     │     │  ├─ base
      │  │  │     │  │     │     │  │  ├─ type: Identifier
      │  │  │     │  │     │     │  │  └─ name: vlp
      │  │  │     │  │     │     │  └─ index
      │  │  │     │  │     │     │     ├─ type: Identifier
      │  │  │     │  │     │     │     └─ name: tokenA
      │  │  │     │  │     │     └─ index
      │  │  │     │  │     │        ├─ type: Identifier
      │  │  │     │  │     │        └─ name: tokenB
      │  │  │     │  │     ├─ 1
      │  │  │     │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  │     │  ├─ variables
      │  │  │     │  │     │  │  └─ 0
      │  │  │     │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     │  │     ├─ typeName
      │  │  │     │  │     │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  │     │  │     │  └─ name: uint
      │  │  │     │  │     │  │     ├─ name: totalVlpA
      │  │  │     │  │     │  │     ├─ storageLocation
      │  │  │     │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     │  │     └─ isIndexed: false
      │  │  │     │  │     │  └─ initialValue
      │  │  │     │  │     │     ├─ type: IndexAccess
      │  │  │     │  │     │     ├─ base
      │  │  │     │  │     │     │  ├─ type: Identifier
      │  │  │     │  │     │     │  └─ name: totalVlp
      │  │  │     │  │     │     └─ index
      │  │  │     │  │     │        ├─ type: MemberAccess
      │  │  │     │  │     │        ├─ expression
      │  │  │     │  │     │        │  ├─ type: Identifier
      │  │  │     │  │     │        │  └─ name: updateData
      │  │  │     │  │     │        └─ memberName: tokenA
      │  │  │     │  │     ├─ 2
      │  │  │     │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  │     │  ├─ variables
      │  │  │     │  │     │  │  └─ 0
      │  │  │     │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     │  │     ├─ typeName
      │  │  │     │  │     │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  │     │  │     │  └─ name: uint
      │  │  │     │  │     │  │     ├─ name: vlpA
      │  │  │     │  │     │  │     ├─ storageLocation
      │  │  │     │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     │  │     └─ isIndexed: false
      │  │  │     │  │     │  └─ initialValue
      │  │  │     │  │     │     ├─ type: FunctionCall
      │  │  │     │  │     │     ├─ expression
      │  │  │     │  │     │     │  ├─ type: Identifier
      │  │  │     │  │     │     │  └─ name: amountToAddVlp
      │  │  │     │  │     │     ├─ arguments
      │  │  │     │  │     │     │  ├─ 0
      │  │  │     │  │     │     │  │  ├─ type: Identifier
      │  │  │     │  │     │     │  │  └─ name: oldVlpA
      │  │  │     │  │     │     │  ├─ 1
      │  │  │     │  │     │     │  │  ├─ type: MemberAccess
      │  │  │     │  │     │     │  │  ├─ expression
      │  │  │     │  │     │     │  │  │  ├─ type: Identifier
      │  │  │     │  │     │     │  │  │  └─ name: updateData
      │  │  │     │  │     │     │  │  └─ memberName: amountA
      │  │  │     │  │     │     │  ├─ 2
      │  │  │     │  │     │     │  │  ├─ type: Identifier
      │  │  │     │  │     │     │  │  └─ name: totalVlpA
      │  │  │     │  │     │     │  └─ 3
      │  │  │     │  │     │     │     ├─ type: Identifier
      │  │  │     │  │     │     │     └─ name: totalReserveA
      │  │  │     │  │     │     └─ names
      │  │  │     │  │     ├─ 3
      │  │  │     │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  │     │  └─ expression
      │  │  │     │  │     │     ├─ type: BinaryOperation
      │  │  │     │  │     │     ├─ operator: =
      │  │  │     │  │     │     ├─ left
      │  │  │     │  │     │     │  ├─ type: IndexAccess
      │  │  │     │  │     │     │  ├─ base
      │  │  │     │  │     │     │  │  ├─ type: IndexAccess
      │  │  │     │  │     │     │  │  ├─ base
      │  │  │     │  │     │     │  │  │  ├─ type: Identifier
      │  │  │     │  │     │     │  │  │  └─ name: vlp
      │  │  │     │  │     │     │  │  └─ index
      │  │  │     │  │     │     │  │     ├─ type: Identifier
      │  │  │     │  │     │     │  │     └─ name: tokenA
      │  │  │     │  │     │     │  └─ index
      │  │  │     │  │     │     │     ├─ type: Identifier
      │  │  │     │  │     │     │     └─ name: tokenB
      │  │  │     │  │     │     └─ right
      │  │  │     │  │     │        ├─ type: Identifier
      │  │  │     │  │     │        └─ name: vlpA
      │  │  │     │  │     └─ 4
      │  │  │     │  │        ├─ type: ExpressionStatement
      │  │  │     │  │        └─ expression
      │  │  │     │  │           ├─ type: BinaryOperation
      │  │  │     │  │           ├─ operator: =
      │  │  │     │  │           ├─ left
      │  │  │     │  │           │  ├─ type: IndexAccess
      │  │  │     │  │           │  ├─ base
      │  │  │     │  │           │  │  ├─ type: Identifier
      │  │  │     │  │           │  │  └─ name: totalVlp
      │  │  │     │  │           │  └─ index
      │  │  │     │  │           │     ├─ type: MemberAccess
      │  │  │     │  │           │     ├─ expression
      │  │  │     │  │           │     │  ├─ type: Identifier
      │  │  │     │  │           │     │  └─ name: updateData
      │  │  │     │  │           │     └─ memberName: tokenA
      │  │  │     │  │           └─ right
      │  │  │     │  │              ├─ type: BinaryOperation
      │  │  │     │  │              ├─ operator: +
      │  │  │     │  │              ├─ left
      │  │  │     │  │              │  ├─ type: BinaryOperation
      │  │  │     │  │              │  ├─ operator: -
      │  │  │     │  │              │  ├─ left
      │  │  │     │  │              │  │  ├─ type: Identifier
      │  │  │     │  │              │  │  └─ name: totalVlpA
      │  │  │     │  │              │  └─ right
      │  │  │     │  │              │     ├─ type: Identifier
      │  │  │     │  │              │     └─ name: oldVlpA
      │  │  │     │  │              └─ right
      │  │  │     │  │                 ├─ type: Identifier
      │  │  │     │  │                 └─ name: vlpA
      │  │  │     │  └─ falseBody
      │  │  │     │     ├─ type: Block
      │  │  │     │     └─ statements
      │  │  │     │        ├─ 0
      │  │  │     │        │  ├─ type: ExpressionStatement
      │  │  │     │        │  └─ expression
      │  │  │     │        │     ├─ type: BinaryOperation
      │  │  │     │        │     ├─ operator: =
      │  │  │     │        │     ├─ left
      │  │  │     │        │     │  ├─ type: IndexAccess
      │  │  │     │        │     │  ├─ base
      │  │  │     │        │     │  │  ├─ type: IndexAccess
      │  │  │     │        │     │  │  ├─ base
      │  │  │     │        │     │  │  │  ├─ type: Identifier
      │  │  │     │        │     │  │  │  └─ name: vlp
      │  │  │     │        │     │  │  └─ index
      │  │  │     │        │     │  │     ├─ type: Identifier
      │  │  │     │        │     │  │     └─ name: tokenA
      │  │  │     │        │     │  └─ index
      │  │  │     │        │     │     ├─ type: Identifier
      │  │  │     │        │     │     └─ name: tokenB
      │  │  │     │        │     └─ right
      │  │  │     │        │        ├─ type: Identifier
      │  │  │     │        │        └─ name: amountA
      │  │  │     │        └─ 1
      │  │  │     │           ├─ type: ExpressionStatement
      │  │  │     │           └─ expression
      │  │  │     │              ├─ type: BinaryOperation
      │  │  │     │              ├─ operator: =
      │  │  │     │              ├─ left
      │  │  │     │              │  ├─ type: IndexAccess
      │  │  │     │              │  ├─ base
      │  │  │     │              │  │  ├─ type: Identifier
      │  │  │     │              │  │  └─ name: totalVlp
      │  │  │     │              │  └─ index
      │  │  │     │              │     ├─ type: MemberAccess
      │  │  │     │              │     ├─ expression
      │  │  │     │              │     │  ├─ type: Identifier
      │  │  │     │              │     │  └─ name: updateData
      │  │  │     │              │     └─ memberName: tokenA
      │  │  │     │              └─ right
      │  │  │     │                 ├─ type: MemberAccess
      │  │  │     │                 ├─ expression
      │  │  │     │                 │  ├─ type: Identifier
      │  │  │     │                 │  └─ name: updateData
      │  │  │     │                 └─ memberName: amountA
      │  │  │     └─ 6
      │  │  │        ├─ type: ExpressionStatement
      │  │  │        └─ expression
      │  │  │           ├─ type: BinaryOperation
      │  │  │           ├─ operator: =
      │  │  │           ├─ left
      │  │  │           │  ├─ type: IndexAccess
      │  │  │           │  ├─ base
      │  │  │           │  │  ├─ type: Identifier
      │  │  │           │  │  └─ name: totalReserve
      │  │  │           │  └─ index
      │  │  │           │     ├─ type: MemberAccess
      │  │  │           │     ├─ expression
      │  │  │           │     │  ├─ type: Identifier
      │  │  │           │     │  └─ name: updateData
      │  │  │           │     └─ memberName: tokenA
      │  │  │           └─ right
      │  │  │              ├─ type: BinaryOperation
      │  │  │              ├─ operator: +
      │  │  │              ├─ left
      │  │  │              │  ├─ type: Identifier
      │  │  │              │  └─ name: totalReserveA
      │  │  │              └─ right
      │  │  │                 ├─ type: MemberAccess
      │  │  │                 ├─ expression
      │  │  │                 │  ├─ type: Identifier
      │  │  │                 │  └─ name: updateData
      │  │  │                 └─ memberName: amountA
      │  │  ├─ visibility: private
      │  │  ├─ modifiers
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability
      │  ├─ 14
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: updateWhenAddLiquidity
      │  │  ├─ parameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: amountA
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  ├─ 1
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: amountB
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  ├─ 2
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: address
      │  │  │  │  ├─ name: tokenA
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 3
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: address
      │  │  │     ├─ name: tokenB
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     ├─ 0
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: updateWhenAddLiquidityOneToken
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: amountA
      │  │  │     │     │  ├─ 1
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: tokenA
      │  │  │     │     │  └─ 2
      │  │  │     │     │     ├─ type: Identifier
      │  │  │     │     │     └─ name: tokenB
      │  │  │     │     └─ names
      │  │  │     └─ 1
      │  │  │        ├─ type: ExpressionStatement
      │  │  │        └─ expression
      │  │  │           ├─ type: FunctionCall
      │  │  │           ├─ expression
      │  │  │           │  ├─ type: Identifier
      │  │  │           │  └─ name: updateWhenAddLiquidityOneToken
      │  │  │           ├─ arguments
      │  │  │           │  ├─ 0
      │  │  │           │  │  ├─ type: Identifier
      │  │  │           │  │  └─ name: amountB
      │  │  │           │  ├─ 1
      │  │  │           │  │  ├─ type: Identifier
      │  │  │           │  │  └─ name: tokenB
      │  │  │           │  └─ 2
      │  │  │           │     ├─ type: Identifier
      │  │  │           │     └─ name: tokenA
      │  │  │           └─ names
      │  │  ├─ visibility: external
      │  │  ├─ modifiers
      │  │  │  └─ 0
      │  │  │     ├─ type: ModifierInvocation
      │  │  │     ├─ name: onlyBank
      │  │  │     └─ arguments
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability
      │  ├─ 15
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: updateWhenRemoveLiquidityOneToken
      │  │  ├─ parameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: amountA
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  ├─ 1
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: address
      │  │  │  │  ├─ name: tokenA
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 2
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: address
      │  │  │     ├─ name: tokenB
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     ├─ 0
      │  │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  ├─ variables
      │  │  │     │  │  └─ 0
      │  │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     ├─ typeName
      │  │  │     │  │     │  ├─ type: UserDefinedTypeName
      │  │  │     │  │     │  └─ namePath: UpdateData
      │  │  │     │  │     ├─ name: updateData
      │  │  │     │  │     ├─ storageLocation: memory
      │  │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     └─ isIndexed: false
      │  │  │     │  └─ initialValue
      │  │  │     ├─ 1
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: MemberAccess
      │  │  │     │     │  ├─ expression
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: updateData
      │  │  │     │     │  └─ memberName: amountA
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: Identifier
      │  │  │     │        └─ name: amountA
      │  │  │     ├─ 2
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: MemberAccess
      │  │  │     │     │  ├─ expression
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: updateData
      │  │  │     │     │  └─ memberName: tokenA
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: Identifier
      │  │  │     │        └─ name: tokenA
      │  │  │     ├─ 3
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: MemberAccess
      │  │  │     │     │  ├─ expression
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: updateData
      │  │  │     │     │  └─ memberName: tokenB
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: Identifier
      │  │  │     │        └─ name: tokenB
      │  │  │     ├─ 4
      │  │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  ├─ variables
      │  │  │     │  │  └─ 0
      │  │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     ├─ typeName
      │  │  │     │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  │     │  └─ name: uint
      │  │  │     │  │     ├─ name: totalReserveA
      │  │  │     │  │     ├─ storageLocation
      │  │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     └─ isIndexed: false
      │  │  │     │  └─ initialValue
      │  │  │     │     ├─ type: IndexAccess
      │  │  │     │     ├─ base
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: totalReserve
      │  │  │     │     └─ index
      │  │  │     │        ├─ type: MemberAccess
      │  │  │     │        ├─ expression
      │  │  │     │        │  ├─ type: Identifier
      │  │  │     │        │  └─ name: updateData
      │  │  │     │        └─ memberName: tokenA
      │  │  │     ├─ 5
      │  │  │     │  ├─ type: IfStatement
      │  │  │     │  ├─ condition
      │  │  │     │  │  ├─ type: BinaryOperation
      │  │  │     │  │  ├─ operator: !=
      │  │  │     │  │  ├─ left
      │  │  │     │  │  │  ├─ type: Identifier
      │  │  │     │  │  │  └─ name: totalReserveA
      │  │  │     │  │  └─ right
      │  │  │     │  │     ├─ type: NumberLiteral
      │  │  │     │  │     ├─ number: 0
      │  │  │     │  │     └─ subdenomination
      │  │  │     │  ├─ trueBody
      │  │  │     │  │  ├─ type: Block
      │  │  │     │  │  └─ statements
      │  │  │     │  │     ├─ 0
      │  │  │     │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  │     │  ├─ variables
      │  │  │     │  │     │  │  └─ 0
      │  │  │     │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     │  │     ├─ typeName
      │  │  │     │  │     │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  │     │  │     │  └─ name: uint
      │  │  │     │  │     │  │     ├─ name: oldVlpA
      │  │  │     │  │     │  │     ├─ storageLocation
      │  │  │     │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     │  │     └─ isIndexed: false
      │  │  │     │  │     │  └─ initialValue
      │  │  │     │  │     │     ├─ type: IndexAccess
      │  │  │     │  │     │     ├─ base
      │  │  │     │  │     │     │  ├─ type: IndexAccess
      │  │  │     │  │     │     │  ├─ base
      │  │  │     │  │     │     │  │  ├─ type: Identifier
      │  │  │     │  │     │     │  │  └─ name: vlp
      │  │  │     │  │     │     │  └─ index
      │  │  │     │  │     │     │     ├─ type: Identifier
      │  │  │     │  │     │     │     └─ name: tokenA
      │  │  │     │  │     │     └─ index
      │  │  │     │  │     │        ├─ type: Identifier
      │  │  │     │  │     │        └─ name: tokenB
      │  │  │     │  │     ├─ 1
      │  │  │     │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  │     │  ├─ variables
      │  │  │     │  │     │  │  └─ 0
      │  │  │     │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     │  │     ├─ typeName
      │  │  │     │  │     │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  │     │  │     │  └─ name: uint
      │  │  │     │  │     │  │     ├─ name: totalVlpA
      │  │  │     │  │     │  │     ├─ storageLocation
      │  │  │     │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     │  │     └─ isIndexed: false
      │  │  │     │  │     │  └─ initialValue
      │  │  │     │  │     │     ├─ type: IndexAccess
      │  │  │     │  │     │     ├─ base
      │  │  │     │  │     │     │  ├─ type: Identifier
      │  │  │     │  │     │     │  └─ name: totalVlp
      │  │  │     │  │     │     └─ index
      │  │  │     │  │     │        ├─ type: MemberAccess
      │  │  │     │  │     │        ├─ expression
      │  │  │     │  │     │        │  ├─ type: Identifier
      │  │  │     │  │     │        │  └─ name: updateData
      │  │  │     │  │     │        └─ memberName: tokenA
      │  │  │     │  │     ├─ 2
      │  │  │     │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  │     │  ├─ variables
      │  │  │     │  │     │  │  └─ 0
      │  │  │     │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     │  │     ├─ typeName
      │  │  │     │  │     │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  │     │  │     │  └─ name: uint
      │  │  │     │  │     │  │     ├─ name: vlpA
      │  │  │     │  │     │  │     ├─ storageLocation
      │  │  │     │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     │  │     └─ isIndexed: false
      │  │  │     │  │     │  └─ initialValue
      │  │  │     │  │     │     ├─ type: FunctionCall
      │  │  │     │  │     │     ├─ expression
      │  │  │     │  │     │     │  ├─ type: Identifier
      │  │  │     │  │     │     │  └─ name: amountToRemoveVlp
      │  │  │     │  │     │     ├─ arguments
      │  │  │     │  │     │     │  ├─ 0
      │  │  │     │  │     │     │  │  ├─ type: Identifier
      │  │  │     │  │     │     │  │  └─ name: oldVlpA
      │  │  │     │  │     │     │  ├─ 1
      │  │  │     │  │     │     │  │  ├─ type: MemberAccess
      │  │  │     │  │     │     │  │  ├─ expression
      │  │  │     │  │     │     │  │  │  ├─ type: Identifier
      │  │  │     │  │     │     │  │  │  └─ name: updateData
      │  │  │     │  │     │     │  │  └─ memberName: amountA
      │  │  │     │  │     │     │  ├─ 2
      │  │  │     │  │     │     │  │  ├─ type: Identifier
      │  │  │     │  │     │     │  │  └─ name: totalVlpA
      │  │  │     │  │     │     │  └─ 3
      │  │  │     │  │     │     │     ├─ type: Identifier
      │  │  │     │  │     │     │     └─ name: totalReserveA
      │  │  │     │  │     │     └─ names
      │  │  │     │  │     ├─ 3
      │  │  │     │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  │     │  └─ expression
      │  │  │     │  │     │     ├─ type: BinaryOperation
      │  │  │     │  │     │     ├─ operator: =
      │  │  │     │  │     │     ├─ left
      │  │  │     │  │     │     │  ├─ type: IndexAccess
      │  │  │     │  │     │     │  ├─ base
      │  │  │     │  │     │     │  │  ├─ type: IndexAccess
      │  │  │     │  │     │     │  │  ├─ base
      │  │  │     │  │     │     │  │  │  ├─ type: Identifier
      │  │  │     │  │     │     │  │  │  └─ name: vlp
      │  │  │     │  │     │     │  │  └─ index
      │  │  │     │  │     │     │  │     ├─ type: Identifier
      │  │  │     │  │     │     │  │     └─ name: tokenA
      │  │  │     │  │     │     │  └─ index
      │  │  │     │  │     │     │     ├─ type: Identifier
      │  │  │     │  │     │     │     └─ name: tokenB
      │  │  │     │  │     │     └─ right
      │  │  │     │  │     │        ├─ type: Identifier
      │  │  │     │  │     │        └─ name: vlpA
      │  │  │     │  │     └─ 4
      │  │  │     │  │        ├─ type: ExpressionStatement
      │  │  │     │  │        └─ expression
      │  │  │     │  │           ├─ type: BinaryOperation
      │  │  │     │  │           ├─ operator: =
      │  │  │     │  │           ├─ left
      │  │  │     │  │           │  ├─ type: IndexAccess
      │  │  │     │  │           │  ├─ base
      │  │  │     │  │           │  │  ├─ type: Identifier
      │  │  │     │  │           │  │  └─ name: totalVlp
      │  │  │     │  │           │  └─ index
      │  │  │     │  │           │     ├─ type: MemberAccess
      │  │  │     │  │           │     ├─ expression
      │  │  │     │  │           │     │  ├─ type: Identifier
      │  │  │     │  │           │     │  └─ name: updateData
      │  │  │     │  │           │     └─ memberName: tokenA
      │  │  │     │  │           └─ right
      │  │  │     │  │              ├─ type: BinaryOperation
      │  │  │     │  │              ├─ operator: +
      │  │  │     │  │              ├─ left
      │  │  │     │  │              │  ├─ type: BinaryOperation
      │  │  │     │  │              │  ├─ operator: -
      │  │  │     │  │              │  ├─ left
      │  │  │     │  │              │  │  ├─ type: Identifier
      │  │  │     │  │              │  │  └─ name: totalVlpA
      │  │  │     │  │              │  └─ right
      │  │  │     │  │              │     ├─ type: Identifier
      │  │  │     │  │              │     └─ name: oldVlpA
      │  │  │     │  │              └─ right
      │  │  │     │  │                 ├─ type: Identifier
      │  │  │     │  │                 └─ name: vlpA
      │  │  │     │  └─ falseBody
      │  │  │     │     ├─ type: Block
      │  │  │     │     └─ statements
      │  │  │     │        ├─ 0
      │  │  │     │        │  ├─ type: ExpressionStatement
      │  │  │     │        │  └─ expression
      │  │  │     │        │     ├─ type: BinaryOperation
      │  │  │     │        │     ├─ operator: =
      │  │  │     │        │     ├─ left
      │  │  │     │        │     │  ├─ type: IndexAccess
      │  │  │     │        │     │  ├─ base
      │  │  │     │        │     │  │  ├─ type: IndexAccess
      │  │  │     │        │     │  │  ├─ base
      │  │  │     │        │     │  │  │  ├─ type: Identifier
      │  │  │     │        │     │  │  │  └─ name: vlp
      │  │  │     │        │     │  │  └─ index
      │  │  │     │        │     │  │     ├─ type: Identifier
      │  │  │     │        │     │  │     └─ name: tokenA
      │  │  │     │        │     │  └─ index
      │  │  │     │        │     │     ├─ type: Identifier
      │  │  │     │        │     │     └─ name: tokenB
      │  │  │     │        │     └─ right
      │  │  │     │        │        ├─ type: Identifier
      │  │  │     │        │        └─ name: amountA
      │  │  │     │        └─ 1
      │  │  │     │           ├─ type: ExpressionStatement
      │  │  │     │           └─ expression
      │  │  │     │              ├─ type: BinaryOperation
      │  │  │     │              ├─ operator: =
      │  │  │     │              ├─ left
      │  │  │     │              │  ├─ type: IndexAccess
      │  │  │     │              │  ├─ base
      │  │  │     │              │  │  ├─ type: Identifier
      │  │  │     │              │  │  └─ name: totalVlp
      │  │  │     │              │  └─ index
      │  │  │     │              │     ├─ type: MemberAccess
      │  │  │     │              │     ├─ expression
      │  │  │     │              │     │  ├─ type: Identifier
      │  │  │     │              │     │  └─ name: updateData
      │  │  │     │              │     └─ memberName: tokenA
      │  │  │     │              └─ right
      │  │  │     │                 ├─ type: MemberAccess
      │  │  │     │                 ├─ expression
      │  │  │     │                 │  ├─ type: Identifier
      │  │  │     │                 │  └─ name: updateData
      │  │  │     │                 └─ memberName: amountA
      │  │  │     └─ 6
      │  │  │        ├─ type: ExpressionStatement
      │  │  │        └─ expression
      │  │  │           ├─ type: BinaryOperation
      │  │  │           ├─ operator: =
      │  │  │           ├─ left
      │  │  │           │  ├─ type: IndexAccess
      │  │  │           │  ├─ base
      │  │  │           │  │  ├─ type: Identifier
      │  │  │           │  │  └─ name: totalReserve
      │  │  │           │  └─ index
      │  │  │           │     ├─ type: MemberAccess
      │  │  │           │     ├─ expression
      │  │  │           │     │  ├─ type: Identifier
      │  │  │           │     │  └─ name: updateData
      │  │  │           │     └─ memberName: tokenA
      │  │  │           └─ right
      │  │  │              ├─ type: BinaryOperation
      │  │  │              ├─ operator: -
      │  │  │              ├─ left
      │  │  │              │  ├─ type: Identifier
      │  │  │              │  └─ name: totalReserveA
      │  │  │              └─ right
      │  │  │                 ├─ type: MemberAccess
      │  │  │                 ├─ expression
      │  │  │                 │  ├─ type: Identifier
      │  │  │                 │  └─ name: updateData
      │  │  │                 └─ memberName: amountA
      │  │  ├─ visibility: private
      │  │  ├─ modifiers
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability
      │  ├─ 16
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: updateWhenRemoveLiquidity
      │  │  ├─ parameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: amount
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 1
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: address
      │  │  │     ├─ name: token
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     ├─ 0
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: require
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  ├─ operator: ==
      │  │  │     │     │  │  ├─ left
      │  │  │     │     │  │  │  ├─ type: MemberAccess
      │  │  │     │     │  │  │  ├─ expression
      │  │  │     │     │  │  │  │  ├─ type: Identifier
      │  │  │     │     │  │  │  │  └─ name: msg
      │  │  │     │     │  │  │  └─ memberName: sender
      │  │  │     │     │  │  └─ right
      │  │  │     │     │  │     ├─ type: Identifier
      │  │  │     │     │  │     └─ name: bankAddress
      │  │  │     │     │  └─ 1
      │  │  │     │     │     ├─ type: StringLiteral
      │  │  │     │     │     ├─ value: APM: Not Authorised
      │  │  │     │     │     └─ parts
      │  │  │     │     │        └─ 0: APM: Not Authorised
      │  │  │     │     └─ names
      │  │  │     └─ 1
      │  │  │        ├─ type: ExpressionStatement
      │  │  │        └─ expression
      │  │  │           ├─ type: BinaryOperation
      │  │  │           ├─ operator: -=
      │  │  │           ├─ left
      │  │  │           │  ├─ type: IndexAccess
      │  │  │           │  ├─ base
      │  │  │           │  │  ├─ type: Identifier
      │  │  │           │  │  └─ name: totalReserve
      │  │  │           │  └─ index
      │  │  │           │     ├─ type: Identifier
      │  │  │           │     └─ name: token
      │  │  │           └─ right
      │  │  │              ├─ type: Identifier
      │  │  │              └─ name: amount
      │  │  ├─ visibility: public
      │  │  ├─ modifiers
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability
      │  ├─ 17
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: updateWhenSwap
      │  │  ├─ parameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: amountAAdded
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  ├─ 1
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: amountBWithdrawn
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  ├─ 2
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: address
      │  │  │  │  ├─ name: tokenA
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 3
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: address
      │  │  │     ├─ name: tokenB
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     ├─ 0
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: updateWhenAddLiquidityOneToken
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: amountAAdded
      │  │  │     │     │  ├─ 1
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: tokenA
      │  │  │     │     │  └─ 2
      │  │  │     │     │     ├─ type: Identifier
      │  │  │     │     │     └─ name: tokenB
      │  │  │     │     └─ names
      │  │  │     └─ 1
      │  │  │        ├─ type: ExpressionStatement
      │  │  │        └─ expression
      │  │  │           ├─ type: FunctionCall
      │  │  │           ├─ expression
      │  │  │           │  ├─ type: Identifier
      │  │  │           │  └─ name: updateWhenRemoveLiquidityOneToken
      │  │  │           ├─ arguments
      │  │  │           │  ├─ 0
      │  │  │           │  │  ├─ type: Identifier
      │  │  │           │  │  └─ name: amountBWithdrawn
      │  │  │           │  ├─ 1
      │  │  │           │  │  ├─ type: Identifier
      │  │  │           │  │  └─ name: tokenB
      │  │  │           │  └─ 2
      │  │  │           │     ├─ type: Identifier
      │  │  │           │     └─ name: tokenA
      │  │  │           └─ names
      │  │  ├─ visibility: private
      │  │  ├─ modifiers
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability
      │  ├─ 18
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: amountToAddVlp
      │  │  ├─ parameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: oldVlp
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  ├─ 1
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: amount
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  ├─ 2
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: totalVlpToken
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 3
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: uint
      │  │  │     ├─ name: totalReserveToken
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  │  └─ 0
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: uint
      │  │  │     ├─ name: newVlp
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     └─ 0
      │  │  │        ├─ type: ExpressionStatement
      │  │  │        └─ expression
      │  │  │           ├─ type: BinaryOperation
      │  │  │           ├─ operator: =
      │  │  │           ├─ left
      │  │  │           │  ├─ type: Identifier
      │  │  │           │  └─ name: newVlp
      │  │  │           └─ right
      │  │  │              ├─ type: BinaryOperation
      │  │  │              ├─ operator: +
      │  │  │              ├─ left
      │  │  │              │  ├─ type: Identifier
      │  │  │              │  └─ name: oldVlp
      │  │  │              └─ right
      │  │  │                 ├─ type: BinaryOperation
      │  │  │                 ├─ operator: /
      │  │  │                 ├─ left
      │  │  │                 │  ├─ type: BinaryOperation
      │  │  │                 │  ├─ operator: *
      │  │  │                 │  ├─ left
      │  │  │                 │  │  ├─ type: Identifier
      │  │  │                 │  │  └─ name: amount
      │  │  │                 │  └─ right
      │  │  │                 │     ├─ type: Identifier
      │  │  │                 │     └─ name: totalVlpToken
      │  │  │                 └─ right
      │  │  │                    ├─ type: Identifier
      │  │  │                    └─ name: totalReserveToken
      │  │  ├─ visibility: public
      │  │  ├─ modifiers
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability: pure
      │  ├─ 19
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: amountToRemoveVlp
      │  │  ├─ parameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: oldVlp
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  ├─ 1
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: amount
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  ├─ 2
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: totalVlpToken
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 3
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: uint
      │  │  │     ├─ name: totalReserveToken
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  │  └─ 0
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: uint
      │  │  │     ├─ name: newVlp
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     └─ 0
      │  │  │        ├─ type: ExpressionStatement
      │  │  │        └─ expression
      │  │  │           ├─ type: BinaryOperation
      │  │  │           ├─ operator: =
      │  │  │           ├─ left
      │  │  │           │  ├─ type: Identifier
      │  │  │           │  └─ name: newVlp
      │  │  │           └─ right
      │  │  │              ├─ type: BinaryOperation
      │  │  │              ├─ operator: -
      │  │  │              ├─ left
      │  │  │              │  ├─ type: Identifier
      │  │  │              │  └─ name: oldVlp
      │  │  │              └─ right
      │  │  │                 ├─ type: BinaryOperation
      │  │  │                 ├─ operator: /
      │  │  │                 ├─ left
      │  │  │                 │  ├─ type: BinaryOperation
      │  │  │                 │  ├─ operator: *
      │  │  │                 │  ├─ left
      │  │  │                 │  │  ├─ type: Identifier
      │  │  │                 │  │  └─ name: amount
      │  │  │                 │  └─ right
      │  │  │                 │     ├─ type: Identifier
      │  │  │                 │     └─ name: totalVlpToken
      │  │  │                 └─ right
      │  │  │                    ├─ type: Identifier
      │  │  │                    └─ name: totalReserveToken
      │  │  ├─ visibility: public
      │  │  ├─ modifiers
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability: pure
      │  ├─ 20
      │  │  ├─ type: StructDefinition
      │  │  ├─ name: SwapData
      │  │  └─ members
      │  │     ├─ 0
      │  │     │  ├─ type: VariableDeclaration
      │  │     │  ├─ typeName
      │  │     │  │  ├─ type: ElementaryTypeName
      │  │     │  │  └─ name: uint
      │  │     │  ├─ name: totalReserve0
      │  │     │  ├─ storageLocation
      │  │     │  ├─ isStateVar: false
      │  │     │  └─ isIndexed: false
      │  │     ├─ 1
      │  │     │  ├─ type: VariableDeclaration
      │  │     │  ├─ typeName
      │  │     │  │  ├─ type: ElementaryTypeName
      │  │     │  │  └─ name: uint
      │  │     │  ├─ name: totalReserve1
      │  │     │  ├─ storageLocation
      │  │     │  ├─ isStateVar: false
      │  │     │  └─ isIndexed: false
      │  │     ├─ 2
      │  │     │  ├─ type: VariableDeclaration
      │  │     │  ├─ typeName
      │  │     │  │  ├─ type: ElementaryTypeName
      │  │     │  │  └─ name: uint
      │  │     │  ├─ name: currentReserve0
      │  │     │  ├─ storageLocation
      │  │     │  ├─ isStateVar: false
      │  │     │  └─ isIndexed: false
      │  │     ├─ 3
      │  │     │  ├─ type: VariableDeclaration
      │  │     │  ├─ typeName
      │  │     │  │  ├─ type: ElementaryTypeName
      │  │     │  │  └─ name: uint
      │  │     │  ├─ name: currentReserve1
      │  │     │  ├─ storageLocation
      │  │     │  ├─ isStateVar: false
      │  │     │  └─ isIndexed: false
      │  │     ├─ 4
      │  │     │  ├─ type: VariableDeclaration
      │  │     │  ├─ typeName
      │  │     │  │  ├─ type: ElementaryTypeName
      │  │     │  │  └─ name: uint
      │  │     │  ├─ name: amount0In
      │  │     │  ├─ storageLocation
      │  │     │  ├─ isStateVar: false
      │  │     │  └─ isIndexed: false
      │  │     └─ 5
      │  │        ├─ type: VariableDeclaration
      │  │        ├─ typeName
      │  │        │  ├─ type: ElementaryTypeName
      │  │        │  └─ name: uint
      │  │        ├─ name: amount1In
      │  │        ├─ storageLocation
      │  │        ├─ isStateVar: false
      │  │        └─ isIndexed: false
      │  ├─ 21
      │  │  ├─ type: StateVariableDeclaration
      │  │  ├─ variables
      │  │  │  └─ 0
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: uint
      │  │  │     ├─ name: unlocked
      │  │  │     ├─ expression
      │  │  │     │  ├─ type: NumberLiteral
      │  │  │     │  ├─ number: 1
      │  │  │     │  └─ subdenomination
      │  │  │     ├─ visibility: private
      │  │  │     ├─ isStateVar: true
      │  │  │     ├─ isDeclaredConst: false
      │  │  │     ├─ isIndexed: false
      │  │  │     ├─ isImmutable: false
      │  │  │     └─ override
      │  │  └─ initialValue
      │  │     ├─ type: NumberLiteral
      │  │     ├─ number: 1
      │  │     └─ subdenomination
      │  ├─ 22
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: swap
      │  │  ├─ parameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: amount0Out
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  ├─ 1
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: amount1Out
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  ├─ 2
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: address
      │  │  │  │  ├─ name: token0
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  ├─ 3
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: address
      │  │  │  │  ├─ name: token1
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 4
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: address
      │  │  │     ├─ name: to
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     ├─ 0
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: require
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  ├─ operator: ==
      │  │  │     │     │  │  ├─ left
      │  │  │     │     │  │  │  ├─ type: Identifier
      │  │  │     │     │  │  │  └─ name: unlocked
      │  │  │     │     │  │  └─ right
      │  │  │     │     │  │     ├─ type: NumberLiteral
      │  │  │     │     │  │     ├─ number: 1
      │  │  │     │     │  │     └─ subdenomination
      │  │  │     │     │  └─ 1
      │  │  │     │     │     ├─ type: StringLiteral
      │  │  │     │     │     ├─ value: APM swap: LOCKED
      │  │  │     │     │     └─ parts
      │  │  │     │     │        └─ 0: APM swap: LOCKED
      │  │  │     │     └─ names
      │  │  │     ├─ 1
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: unlocked
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: NumberLiteral
      │  │  │     │        ├─ number: 0
      │  │  │     │        └─ subdenomination
      │  │  │     ├─ 2
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: require
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  ├─ operator: ||
      │  │  │     │     │  │  ├─ left
      │  │  │     │     │  │  │  ├─ type: TupleExpression
      │  │  │     │     │  │  │  ├─ components
      │  │  │     │     │  │  │  │  └─ 0
      │  │  │     │     │  │  │  │     ├─ type: BinaryOperation
      │  │  │     │     │  │  │  │     ├─ operator: &&
      │  │  │     │     │  │  │  │     ├─ left
      │  │  │     │     │  │  │  │     │  ├─ type: BinaryOperation
      │  │  │     │     │  │  │  │     │  ├─ operator: !=
      │  │  │     │     │  │  │  │     │  ├─ left
      │  │  │     │     │  │  │  │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  │  │     │  │  └─ name: amount0Out
      │  │  │     │     │  │  │  │     │  └─ right
      │  │  │     │     │  │  │  │     │     ├─ type: NumberLiteral
      │  │  │     │     │  │  │  │     │     ├─ number: 0
      │  │  │     │     │  │  │  │     │     └─ subdenomination
      │  │  │     │     │  │  │  │     └─ right
      │  │  │     │     │  │  │  │        ├─ type: BinaryOperation
      │  │  │     │     │  │  │  │        ├─ operator: ==
      │  │  │     │     │  │  │  │        ├─ left
      │  │  │     │     │  │  │  │        │  ├─ type: Identifier
      │  │  │     │     │  │  │  │        │  └─ name: amount1Out
      │  │  │     │     │  │  │  │        └─ right
      │  │  │     │     │  │  │  │           ├─ type: NumberLiteral
      │  │  │     │     │  │  │  │           ├─ number: 0
      │  │  │     │     │  │  │  │           └─ subdenomination
      │  │  │     │     │  │  │  └─ isArray: false
      │  │  │     │     │  │  └─ right
      │  │  │     │     │  │     ├─ type: TupleExpression
      │  │  │     │     │  │     ├─ components
      │  │  │     │     │  │     │  └─ 0
      │  │  │     │     │  │     │     ├─ type: BinaryOperation
      │  │  │     │     │  │     │     ├─ operator: &&
      │  │  │     │     │  │     │     ├─ left
      │  │  │     │     │  │     │     │  ├─ type: BinaryOperation
      │  │  │     │     │  │     │     │  ├─ operator: ==
      │  │  │     │     │  │     │     │  ├─ left
      │  │  │     │     │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │     │     │  │  └─ name: amount0Out
      │  │  │     │     │  │     │     │  └─ right
      │  │  │     │     │  │     │     │     ├─ type: NumberLiteral
      │  │  │     │     │  │     │     │     ├─ number: 0
      │  │  │     │     │  │     │     │     └─ subdenomination
      │  │  │     │     │  │     │     └─ right
      │  │  │     │     │  │     │        ├─ type: BinaryOperation
      │  │  │     │     │  │     │        ├─ operator: !=
      │  │  │     │     │  │     │        ├─ left
      │  │  │     │     │  │     │        │  ├─ type: Identifier
      │  │  │     │     │  │     │        │  └─ name: amount1Out
      │  │  │     │     │  │     │        └─ right
      │  │  │     │     │  │     │           ├─ type: NumberLiteral
      │  │  │     │     │  │     │           ├─ number: 0
      │  │  │     │     │  │     │           └─ subdenomination
      │  │  │     │     │  │     └─ isArray: false
      │  │  │     │     │  └─ 1
      │  │  │     │     │     ├─ type: StringLiteral
      │  │  │     │     │     ├─ value: APM swap: INSUFFICIENT_OUTPUT_AMOUNT_Or_Both_output >0
      │  │  │     │     │     └─ parts
      │  │  │     │     │        └─ 0: APM swap: INSUFFICIENT_OUTPUT_AMOUNT_Or_Both_output >0
      │  │  │     │     └─ names
      │  │  │     ├─ 3
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: require
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  ├─ operator: &&
      │  │  │     │     │  │  ├─ left
      │  │  │     │     │  │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  │  ├─ operator: !=
      │  │  │     │     │  │  │  ├─ left
      │  │  │     │     │  │  │  │  ├─ type: Identifier
      │  │  │     │     │  │  │  │  └─ name: to
      │  │  │     │     │  │  │  └─ right
      │  │  │     │     │  │  │     ├─ type: Identifier
      │  │  │     │     │  │  │     └─ name: token0
      │  │  │     │     │  │  └─ right
      │  │  │     │     │  │     ├─ type: BinaryOperation
      │  │  │     │     │  │     ├─ operator: !=
      │  │  │     │     │  │     ├─ left
      │  │  │     │     │  │     │  ├─ type: Identifier
      │  │  │     │     │  │     │  └─ name: to
      │  │  │     │     │  │     └─ right
      │  │  │     │     │  │        ├─ type: Identifier
      │  │  │     │     │  │        └─ name: token1
      │  │  │     │     │  └─ 1
      │  │  │     │     │     ├─ type: StringLiteral
      │  │  │     │     │     ├─ value: APM swap: INVALID_TO
      │  │  │     │     │     └─ parts
      │  │  │     │     │        └─ 0: APM swap: INVALID_TO
      │  │  │     │     └─ names
      │  │  │     ├─ 4
      │  │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  ├─ variables
      │  │  │     │  │  ├─ 0
      │  │  │     │  │  │  ├─ type: VariableDeclaration
      │  │  │     │  │  │  ├─ name: _reserve0
      │  │  │     │  │  │  ├─ typeName
      │  │  │     │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │     │  │  │  │  └─ name: uint
      │  │  │     │  │  │  ├─ storageLocation
      │  │  │     │  │  │  ├─ isStateVar: false
      │  │  │     │  │  │  └─ isIndexed: false
      │  │  │     │  │  └─ 1
      │  │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     ├─ name: _reserve1
      │  │  │     │  │     ├─ typeName
      │  │  │     │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  │     │  └─ name: uint
      │  │  │     │  │     ├─ storageLocation
      │  │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     └─ isIndexed: false
      │  │  │     │  └─ initialValue
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: getReserves
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: token0
      │  │  │     │     │  └─ 1
      │  │  │     │     │     ├─ type: Identifier
      │  │  │     │     │     └─ name: token1
      │  │  │     │     └─ names
      │  │  │     ├─ 5
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: require
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  ├─ operator: &&
      │  │  │     │     │  │  ├─ left
      │  │  │     │     │  │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  │  ├─ operator: <
      │  │  │     │     │  │  │  ├─ left
      │  │  │     │     │  │  │  │  ├─ type: Identifier
      │  │  │     │     │  │  │  │  └─ name: amount0Out
      │  │  │     │     │  │  │  └─ right
      │  │  │     │     │  │  │     ├─ type: Identifier
      │  │  │     │     │  │  │     └─ name: _reserve0
      │  │  │     │     │  │  └─ right
      │  │  │     │     │  │     ├─ type: BinaryOperation
      │  │  │     │     │  │     ├─ operator: <
      │  │  │     │     │  │     ├─ left
      │  │  │     │     │  │     │  ├─ type: Identifier
      │  │  │     │     │  │     │  └─ name: amount1Out
      │  │  │     │     │  │     └─ right
      │  │  │     │     │  │        ├─ type: Identifier
      │  │  │     │     │  │        └─ name: _reserve1
      │  │  │     │     │  └─ 1
      │  │  │     │     │     ├─ type: StringLiteral
      │  │  │     │     │     ├─ value: APM swap: INSUFFICIENT_LIQUIDITY
      │  │  │     │     │     └─ parts
      │  │  │     │     │        └─ 0: APM swap: INSUFFICIENT_LIQUIDITY
      │  │  │     │     └─ names
      │  │  │     ├─ 6
      │  │  │     │  ├─ type: IfStatement
      │  │  │     │  ├─ condition
      │  │  │     │  │  ├─ type: BinaryOperation
      │  │  │     │  │  ├─ operator: ==
      │  │  │     │  │  ├─ left
      │  │  │     │  │  │  ├─ type: Identifier
      │  │  │     │  │  │  └─ name: amount0Out
      │  │  │     │  │  └─ right
      │  │  │     │  │     ├─ type: NumberLiteral
      │  │  │     │  │     ├─ number: 0
      │  │  │     │  │     └─ subdenomination
      │  │  │     │  ├─ trueBody
      │  │  │     │  │  ├─ type: ExpressionStatement
      │  │  │     │  │  └─ expression
      │  │  │     │  │     ├─ type: FunctionCall
      │  │  │     │  │     ├─ expression
      │  │  │     │  │     │  ├─ type: MemberAccess
      │  │  │     │  │     │  ├─ expression
      │  │  │     │  │     │  │  ├─ type: FunctionCall
      │  │  │     │  │     │  │  ├─ expression
      │  │  │     │  │     │  │  │  ├─ type: Identifier
      │  │  │     │  │     │  │  │  └─ name: IERC20
      │  │  │     │  │     │  │  ├─ arguments
      │  │  │     │  │     │  │  │  └─ 0
      │  │  │     │  │     │  │  │     ├─ type: Identifier
      │  │  │     │  │     │  │  │     └─ name: token1
      │  │  │     │  │     │  │  └─ names
      │  │  │     │  │     │  └─ memberName: transfer
      │  │  │     │  │     ├─ arguments
      │  │  │     │  │     │  ├─ 0
      │  │  │     │  │     │  │  ├─ type: Identifier
      │  │  │     │  │     │  │  └─ name: to
      │  │  │     │  │     │  └─ 1
      │  │  │     │  │     │     ├─ type: Identifier
      │  │  │     │  │     │     └─ name: amount1Out
      │  │  │     │  │     └─ names
      │  │  │     │  └─ falseBody
      │  │  │     │     ├─ type: ExpressionStatement
      │  │  │     │     └─ expression
      │  │  │     │        ├─ type: FunctionCall
      │  │  │     │        ├─ expression
      │  │  │     │        │  ├─ type: MemberAccess
      │  │  │     │        │  ├─ expression
      │  │  │     │        │  │  ├─ type: FunctionCall
      │  │  │     │        │  │  ├─ expression
      │  │  │     │        │  │  │  ├─ type: Identifier
      │  │  │     │        │  │  │  └─ name: IERC20
      │  │  │     │        │  │  ├─ arguments
      │  │  │     │        │  │  │  └─ 0
      │  │  │     │        │  │  │     ├─ type: Identifier
      │  │  │     │        │  │  │     └─ name: token0
      │  │  │     │        │  │  └─ names
      │  │  │     │        │  └─ memberName: transfer
      │  │  │     │        ├─ arguments
      │  │  │     │        │  ├─ 0
      │  │  │     │        │  │  ├─ type: Identifier
      │  │  │     │        │  │  └─ name: to
      │  │  │     │        │  └─ 1
      │  │  │     │        │     ├─ type: Identifier
      │  │  │     │        │     └─ name: amount0Out
      │  │  │     │        └─ names
      │  │  │     ├─ 7
      │  │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  ├─ variables
      │  │  │     │  │  └─ 0
      │  │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     ├─ typeName
      │  │  │     │  │     │  ├─ type: UserDefinedTypeName
      │  │  │     │  │     │  └─ namePath: SwapData
      │  │  │     │  │     ├─ name: swapData
      │  │  │     │  │     ├─ storageLocation: memory
      │  │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     └─ isIndexed: false
      │  │  │     │  └─ initialValue
      │  │  │     ├─ 8
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: MemberAccess
      │  │  │     │     │  ├─ expression
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: swapData
      │  │  │     │     │  └─ memberName: totalReserve0
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: FunctionCall
      │  │  │     │        ├─ expression
      │  │  │     │        │  ├─ type: MemberAccess
      │  │  │     │        │  ├─ expression
      │  │  │     │        │  │  ├─ type: FunctionCall
      │  │  │     │        │  │  ├─ expression
      │  │  │     │        │  │  │  ├─ type: Identifier
      │  │  │     │        │  │  │  └─ name: IERC20
      │  │  │     │        │  │  ├─ arguments
      │  │  │     │        │  │  │  └─ 0
      │  │  │     │        │  │  │     ├─ type: Identifier
      │  │  │     │        │  │  │     └─ name: token0
      │  │  │     │        │  │  └─ names
      │  │  │     │        │  └─ memberName: balanceOf
      │  │  │     │        ├─ arguments
      │  │  │     │        │  └─ 0
      │  │  │     │        │     ├─ type: FunctionCall
      │  │  │     │        │     ├─ expression
      │  │  │     │        │     │  ├─ type: TypeNameExpression
      │  │  │     │        │     │  └─ typeName
      │  │  │     │        │     │     ├─ type: ElementaryTypeName
      │  │  │     │        │     │     └─ name: address
      │  │  │     │        │     ├─ arguments
      │  │  │     │        │     │  └─ 0
      │  │  │     │        │     │     ├─ type: Identifier
      │  │  │     │        │     │     └─ name: this
      │  │  │     │        │     └─ names
      │  │  │     │        └─ names
      │  │  │     ├─ 9
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: MemberAccess
      │  │  │     │     │  ├─ expression
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: swapData
      │  │  │     │     │  └─ memberName: totalReserve1
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: FunctionCall
      │  │  │     │        ├─ expression
      │  │  │     │        │  ├─ type: MemberAccess
      │  │  │     │        │  ├─ expression
      │  │  │     │        │  │  ├─ type: FunctionCall
      │  │  │     │        │  │  ├─ expression
      │  │  │     │        │  │  │  ├─ type: Identifier
      │  │  │     │        │  │  │  └─ name: IERC20
      │  │  │     │        │  │  ├─ arguments
      │  │  │     │        │  │  │  └─ 0
      │  │  │     │        │  │  │     ├─ type: Identifier
      │  │  │     │        │  │  │     └─ name: token1
      │  │  │     │        │  │  └─ names
      │  │  │     │        │  └─ memberName: balanceOf
      │  │  │     │        ├─ arguments
      │  │  │     │        │  └─ 0
      │  │  │     │        │     ├─ type: FunctionCall
      │  │  │     │        │     ├─ expression
      │  │  │     │        │     │  ├─ type: TypeNameExpression
      │  │  │     │        │     │  └─ typeName
      │  │  │     │        │     │     ├─ type: ElementaryTypeName
      │  │  │     │        │     │     └─ name: address
      │  │  │     │        │     ├─ arguments
      │  │  │     │        │     │  └─ 0
      │  │  │     │        │     │     ├─ type: Identifier
      │  │  │     │        │     │     └─ name: this
      │  │  │     │        │     └─ names
      │  │  │     │        └─ names
      │  │  │     ├─ 10
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: MemberAccess
      │  │  │     │     │  ├─ expression
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: swapData
      │  │  │     │     │  └─ memberName: currentReserve0
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: BinaryOperation
      │  │  │     │        ├─ operator: -
      │  │  │     │        ├─ left
      │  │  │     │        │  ├─ type: BinaryOperation
      │  │  │     │        │  ├─ operator: +
      │  │  │     │        │  ├─ left
      │  │  │     │        │  │  ├─ type: Identifier
      │  │  │     │        │  │  └─ name: _reserve0
      │  │  │     │        │  └─ right
      │  │  │     │        │     ├─ type: MemberAccess
      │  │  │     │        │     ├─ expression
      │  │  │     │        │     │  ├─ type: Identifier
      │  │  │     │        │     │  └─ name: swapData
      │  │  │     │        │     └─ memberName: totalReserve0
      │  │  │     │        └─ right
      │  │  │     │           ├─ type: IndexAccess
      │  │  │     │           ├─ base
      │  │  │     │           │  ├─ type: Identifier
      │  │  │     │           │  └─ name: totalReserve
      │  │  │     │           └─ index
      │  │  │     │              ├─ type: Identifier
      │  │  │     │              └─ name: token0
      │  │  │     ├─ 11
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: MemberAccess
      │  │  │     │     │  ├─ expression
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: swapData
      │  │  │     │     │  └─ memberName: currentReserve1
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: BinaryOperation
      │  │  │     │        ├─ operator: -
      │  │  │     │        ├─ left
      │  │  │     │        │  ├─ type: BinaryOperation
      │  │  │     │        │  ├─ operator: +
      │  │  │     │        │  ├─ left
      │  │  │     │        │  │  ├─ type: Identifier
      │  │  │     │        │  │  └─ name: _reserve1
      │  │  │     │        │  └─ right
      │  │  │     │        │     ├─ type: MemberAccess
      │  │  │     │        │     ├─ expression
      │  │  │     │        │     │  ├─ type: Identifier
      │  │  │     │        │     │  └─ name: swapData
      │  │  │     │        │     └─ memberName: totalReserve1
      │  │  │     │        └─ right
      │  │  │     │           ├─ type: IndexAccess
      │  │  │     │           ├─ base
      │  │  │     │           │  ├─ type: Identifier
      │  │  │     │           │  └─ name: totalReserve
      │  │  │     │           └─ index
      │  │  │     │              ├─ type: Identifier
      │  │  │     │              └─ name: token1
      │  │  │     ├─ 12
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: require
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  ├─ operator: >=
      │  │  │     │     │  │  ├─ left
      │  │  │     │     │  │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  │  ├─ operator: *
      │  │  │     │     │  │  │  ├─ left
      │  │  │     │     │  │  │  │  ├─ type: MemberAccess
      │  │  │     │     │  │  │  │  ├─ expression
      │  │  │     │     │  │  │  │  │  ├─ type: Identifier
      │  │  │     │     │  │  │  │  │  └─ name: swapData
      │  │  │     │     │  │  │  │  └─ memberName: currentReserve0
      │  │  │     │     │  │  │  └─ right
      │  │  │     │     │  │  │     ├─ type: MemberAccess
      │  │  │     │     │  │  │     ├─ expression
      │  │  │     │     │  │  │     │  ├─ type: Identifier
      │  │  │     │     │  │  │     │  └─ name: swapData
      │  │  │     │     │  │  │     └─ memberName: currentReserve1
      │  │  │     │     │  │  └─ right
      │  │  │     │     │  │     ├─ type: BinaryOperation
      │  │  │     │     │  │     ├─ operator: *
      │  │  │     │     │  │     ├─ left
      │  │  │     │     │  │     │  ├─ type: Identifier
      │  │  │     │     │  │     │  └─ name: _reserve0
      │  │  │     │     │  │     └─ right
      │  │  │     │     │  │        ├─ type: Identifier
      │  │  │     │     │  │        └─ name: _reserve1
      │  │  │     │     │  └─ 1
      │  │  │     │     │     ├─ type: StringLiteral
      │  │  │     │     │     ├─ value: APM swap: K
      │  │  │     │     │     └─ parts
      │  │  │     │     │        └─ 0: APM swap: K
      │  │  │     │     └─ names
      │  │  │     ├─ 13
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: MemberAccess
      │  │  │     │     │  ├─ expression
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: swapData
      │  │  │     │     │  └─ memberName: amount0In
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: Conditional
      │  │  │     │        ├─ condition
      │  │  │     │        │  ├─ type: BinaryOperation
      │  │  │     │        │  ├─ operator: >
      │  │  │     │        │  ├─ left
      │  │  │     │        │  │  ├─ type: MemberAccess
      │  │  │     │        │  │  ├─ expression
      │  │  │     │        │  │  │  ├─ type: Identifier
      │  │  │     │        │  │  │  └─ name: swapData
      │  │  │     │        │  │  └─ memberName: currentReserve0
      │  │  │     │        │  └─ right
      │  │  │     │        │     ├─ type: BinaryOperation
      │  │  │     │        │     ├─ operator: -
      │  │  │     │        │     ├─ left
      │  │  │     │        │     │  ├─ type: Identifier
      │  │  │     │        │     │  └─ name: _reserve0
      │  │  │     │        │     └─ right
      │  │  │     │        │        ├─ type: Identifier
      │  │  │     │        │        └─ name: amount0Out
      │  │  │     │        ├─ trueExpression
      │  │  │     │        │  ├─ type: BinaryOperation
      │  │  │     │        │  ├─ operator: -
      │  │  │     │        │  ├─ left
      │  │  │     │        │  │  ├─ type: MemberAccess
      │  │  │     │        │  │  ├─ expression
      │  │  │     │        │  │  │  ├─ type: Identifier
      │  │  │     │        │  │  │  └─ name: swapData
      │  │  │     │        │  │  └─ memberName: currentReserve0
      │  │  │     │        │  └─ right
      │  │  │     │        │     ├─ type: TupleExpression
      │  │  │     │        │     ├─ components
      │  │  │     │        │     │  └─ 0
      │  │  │     │        │     │     ├─ type: BinaryOperation
      │  │  │     │        │     │     ├─ operator: -
      │  │  │     │        │     │     ├─ left
      │  │  │     │        │     │     │  ├─ type: Identifier
      │  │  │     │        │     │     │  └─ name: _reserve0
      │  │  │     │        │     │     └─ right
      │  │  │     │        │     │        ├─ type: Identifier
      │  │  │     │        │     │        └─ name: amount0Out
      │  │  │     │        │     └─ isArray: false
      │  │  │     │        └─ falseExpression
      │  │  │     │           ├─ type: NumberLiteral
      │  │  │     │           ├─ number: 0
      │  │  │     │           └─ subdenomination
      │  │  │     ├─ 14
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: MemberAccess
      │  │  │     │     │  ├─ expression
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: swapData
      │  │  │     │     │  └─ memberName: amount1In
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: Conditional
      │  │  │     │        ├─ condition
      │  │  │     │        │  ├─ type: BinaryOperation
      │  │  │     │        │  ├─ operator: >
      │  │  │     │        │  ├─ left
      │  │  │     │        │  │  ├─ type: MemberAccess
      │  │  │     │        │  │  ├─ expression
      │  │  │     │        │  │  │  ├─ type: Identifier
      │  │  │     │        │  │  │  └─ name: swapData
      │  │  │     │        │  │  └─ memberName: currentReserve1
      │  │  │     │        │  └─ right
      │  │  │     │        │     ├─ type: BinaryOperation
      │  │  │     │        │     ├─ operator: -
      │  │  │     │        │     ├─ left
      │  │  │     │        │     │  ├─ type: Identifier
      │  │  │     │        │     │  └─ name: _reserve1
      │  │  │     │        │     └─ right
      │  │  │     │        │        ├─ type: Identifier
      │  │  │     │        │        └─ name: amount1Out
      │  │  │     │        ├─ trueExpression
      │  │  │     │        │  ├─ type: BinaryOperation
      │  │  │     │        │  ├─ operator: -
      │  │  │     │        │  ├─ left
      │  │  │     │        │  │  ├─ type: MemberAccess
      │  │  │     │        │  │  ├─ expression
      │  │  │     │        │  │  │  ├─ type: Identifier
      │  │  │     │        │  │  │  └─ name: swapData
      │  │  │     │        │  │  └─ memberName: currentReserve1
      │  │  │     │        │  └─ right
      │  │  │     │        │     ├─ type: TupleExpression
      │  │  │     │        │     ├─ components
      │  │  │     │        │     │  └─ 0
      │  │  │     │        │     │     ├─ type: BinaryOperation
      │  │  │     │        │     │     ├─ operator: -
      │  │  │     │        │     │     ├─ left
      │  │  │     │        │     │     │  ├─ type: Identifier
      │  │  │     │        │     │     │  └─ name: _reserve1
      │  │  │     │        │     │     └─ right
      │  │  │     │        │     │        ├─ type: Identifier
      │  │  │     │        │     │        └─ name: amount1Out
      │  │  │     │        │     └─ isArray: false
      │  │  │     │        └─ falseExpression
      │  │  │     │           ├─ type: NumberLiteral
      │  │  │     │           ├─ number: 0
      │  │  │     │           └─ subdenomination
      │  │  │     ├─ 15
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: require
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  ├─ operator: ||
      │  │  │     │     │  │  ├─ left
      │  │  │     │     │  │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  │  ├─ operator: >
      │  │  │     │     │  │  │  ├─ left
      │  │  │     │     │  │  │  │  ├─ type: MemberAccess
      │  │  │     │     │  │  │  │  ├─ expression
      │  │  │     │     │  │  │  │  │  ├─ type: Identifier
      │  │  │     │     │  │  │  │  │  └─ name: swapData
      │  │  │     │     │  │  │  │  └─ memberName: amount0In
      │  │  │     │     │  │  │  └─ right
      │  │  │     │     │  │  │     ├─ type: NumberLiteral
      │  │  │     │     │  │  │     ├─ number: 0
      │  │  │     │     │  │  │     └─ subdenomination
      │  │  │     │     │  │  └─ right
      │  │  │     │     │  │     ├─ type: BinaryOperation
      │  │  │     │     │  │     ├─ operator: >
      │  │  │     │     │  │     ├─ left
      │  │  │     │     │  │     │  ├─ type: MemberAccess
      │  │  │     │     │  │     │  ├─ expression
      │  │  │     │     │  │     │  │  ├─ type: Identifier
      │  │  │     │     │  │     │  │  └─ name: swapData
      │  │  │     │     │  │     │  └─ memberName: amount1In
      │  │  │     │     │  │     └─ right
      │  │  │     │     │  │        ├─ type: NumberLiteral
      │  │  │     │     │  │        ├─ number: 0
      │  │  │     │     │  │        └─ subdenomination
      │  │  │     │     │  └─ 1
      │  │  │     │     │     ├─ type: StringLiteral
      │  │  │     │     │     ├─ value: APM swap: INSUFFICIENT_INPUT_AMOUNT
      │  │  │     │     │     └─ parts
      │  │  │     │     │        └─ 0: APM swap: INSUFFICIENT_INPUT_AMOUNT
      │  │  │     │     └─ names
      │  │  │     ├─ 16
      │  │  │     │  ├─ type: IfStatement
      │  │  │     │  ├─ condition
      │  │  │     │  │  ├─ type: BinaryOperation
      │  │  │     │  │  ├─ operator: ==
      │  │  │     │  │  ├─ left
      │  │  │     │  │  │  ├─ type: Identifier
      │  │  │     │  │  │  └─ name: amount0Out
      │  │  │     │  │  └─ right
      │  │  │     │  │     ├─ type: NumberLiteral
      │  │  │     │  │     ├─ number: 0
      │  │  │     │  │     └─ subdenomination
      │  │  │     │  ├─ trueBody
      │  │  │     │  │  ├─ type: Block
      │  │  │     │  │  └─ statements
      │  │  │     │  │     └─ 0
      │  │  │     │  │        ├─ type: ExpressionStatement
      │  │  │     │  │        └─ expression
      │  │  │     │  │           ├─ type: FunctionCall
      │  │  │     │  │           ├─ expression
      │  │  │     │  │           │  ├─ type: Identifier
      │  │  │     │  │           │  └─ name: updateWhenSwap
      │  │  │     │  │           ├─ arguments
      │  │  │     │  │           │  ├─ 0
      │  │  │     │  │           │  │  ├─ type: MemberAccess
      │  │  │     │  │           │  │  ├─ expression
      │  │  │     │  │           │  │  │  ├─ type: Identifier
      │  │  │     │  │           │  │  │  └─ name: swapData
      │  │  │     │  │           │  │  └─ memberName: amount0In
      │  │  │     │  │           │  ├─ 1
      │  │  │     │  │           │  │  ├─ type: Identifier
      │  │  │     │  │           │  │  └─ name: amount1Out
      │  │  │     │  │           │  ├─ 2
      │  │  │     │  │           │  │  ├─ type: Identifier
      │  │  │     │  │           │  │  └─ name: token0
      │  │  │     │  │           │  └─ 3
      │  │  │     │  │           │     ├─ type: Identifier
      │  │  │     │  │           │     └─ name: token1
      │  │  │     │  │           └─ names
      │  │  │     │  └─ falseBody
      │  │  │     │     ├─ type: Block
      │  │  │     │     └─ statements
      │  │  │     │        └─ 0
      │  │  │     │           ├─ type: ExpressionStatement
      │  │  │     │           └─ expression
      │  │  │     │              ├─ type: FunctionCall
      │  │  │     │              ├─ expression
      │  │  │     │              │  ├─ type: Identifier
      │  │  │     │              │  └─ name: updateWhenSwap
      │  │  │     │              ├─ arguments
      │  │  │     │              │  ├─ 0
      │  │  │     │              │  │  ├─ type: MemberAccess
      │  │  │     │              │  │  ├─ expression
      │  │  │     │              │  │  │  ├─ type: Identifier
      │  │  │     │              │  │  │  └─ name: swapData
      │  │  │     │              │  │  └─ memberName: amount1In
      │  │  │     │              │  ├─ 1
      │  │  │     │              │  │  ├─ type: Identifier
      │  │  │     │              │  │  └─ name: amount0Out
      │  │  │     │              │  ├─ 2
      │  │  │     │              │  │  ├─ type: Identifier
      │  │  │     │              │  │  └─ name: token1
      │  │  │     │              │  └─ 3
      │  │  │     │              │     ├─ type: Identifier
      │  │  │     │              │     └─ name: token0
      │  │  │     │              └─ names
      │  │  │     └─ 17
      │  │  │        ├─ type: ExpressionStatement
      │  │  │        └─ expression
      │  │  │           ├─ type: BinaryOperation
      │  │  │           ├─ operator: =
      │  │  │           ├─ left
      │  │  │           │  ├─ type: Identifier
      │  │  │           │  └─ name: unlocked
      │  │  │           └─ right
      │  │  │              ├─ type: NumberLiteral
      │  │  │              ├─ number: 1
      │  │  │              └─ subdenomination
      │  │  ├─ visibility: external
      │  │  ├─ modifiers
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability
      │  ├─ 23
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: getAmountOut
      │  │  ├─ parameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: amountIn
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  ├─ 1
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: reserveIn
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 2
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: uint
      │  │  │     ├─ name: reserveOut
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  │  └─ 0
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  └─ name: uint
      │  │  │     ├─ name: amountOut
      │  │  │     ├─ storageLocation
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     ├─ 0
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: require
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  ├─ operator: >
      │  │  │     │     │  │  ├─ left
      │  │  │     │     │  │  │  ├─ type: Identifier
      │  │  │     │     │  │  │  └─ name: amountIn
      │  │  │     │     │  │  └─ right
      │  │  │     │     │  │     ├─ type: NumberLiteral
      │  │  │     │     │  │     ├─ number: 0
      │  │  │     │     │  │     └─ subdenomination
      │  │  │     │     │  └─ 1
      │  │  │     │     │     ├─ type: StringLiteral
      │  │  │     │     │     ├─ value: APM: INSUFFICIENT_INPUT_AMOUNT
      │  │  │     │     │     └─ parts
      │  │  │     │     │        └─ 0: APM: INSUFFICIENT_INPUT_AMOUNT
      │  │  │     │     └─ names
      │  │  │     ├─ 1
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: require
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  ├─ operator: &&
      │  │  │     │     │  │  ├─ left
      │  │  │     │     │  │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  │  ├─ operator: >
      │  │  │     │     │  │  │  ├─ left
      │  │  │     │     │  │  │  │  ├─ type: Identifier
      │  │  │     │     │  │  │  │  └─ name: reserveIn
      │  │  │     │     │  │  │  └─ right
      │  │  │     │     │  │  │     ├─ type: NumberLiteral
      │  │  │     │     │  │  │     ├─ number: 0
      │  │  │     │     │  │  │     └─ subdenomination
      │  │  │     │     │  │  └─ right
      │  │  │     │     │  │     ├─ type: BinaryOperation
      │  │  │     │     │  │     ├─ operator: >
      │  │  │     │     │  │     ├─ left
      │  │  │     │     │  │     │  ├─ type: Identifier
      │  │  │     │     │  │     │  └─ name: reserveOut
      │  │  │     │     │  │     └─ right
      │  │  │     │     │  │        ├─ type: NumberLiteral
      │  │  │     │     │  │        ├─ number: 0
      │  │  │     │     │  │        └─ subdenomination
      │  │  │     │     │  └─ 1
      │  │  │     │     │     ├─ type: StringLiteral
      │  │  │     │     │     ├─ value: APM: INSUFFICIENT_LIQUIDITY
      │  │  │     │     │     └─ parts
      │  │  │     │     │        └─ 0: APM: INSUFFICIENT_LIQUIDITY
      │  │  │     │     └─ names
      │  │  │     ├─ 2
      │  │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  ├─ variables
      │  │  │     │  │  └─ 0
      │  │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     ├─ typeName
      │  │  │     │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  │     │  └─ name: uint
      │  │  │     │  │     ├─ name: numerator
      │  │  │     │  │     ├─ storageLocation
      │  │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     └─ isIndexed: false
      │  │  │     │  └─ initialValue
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: *
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: amountIn
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: Identifier
      │  │  │     │        └─ name: reserveOut
      │  │  │     ├─ 3
      │  │  │     │  ├─ type: VariableDeclarationStatement
      │  │  │     │  ├─ variables
      │  │  │     │  │  └─ 0
      │  │  │     │  │     ├─ type: VariableDeclaration
      │  │  │     │  │     ├─ typeName
      │  │  │     │  │     │  ├─ type: ElementaryTypeName
      │  │  │     │  │     │  └─ name: uint
      │  │  │     │  │     ├─ name: denominator
      │  │  │     │  │     ├─ storageLocation
      │  │  │     │  │     ├─ isStateVar: false
      │  │  │     │  │     └─ isIndexed: false
      │  │  │     │  └─ initialValue
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: +
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: reserveIn
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: Identifier
      │  │  │     │        └─ name: amountIn
      │  │  │     └─ 4
      │  │  │        ├─ type: ExpressionStatement
      │  │  │        └─ expression
      │  │  │           ├─ type: BinaryOperation
      │  │  │           ├─ operator: =
      │  │  │           ├─ left
      │  │  │           │  ├─ type: Identifier
      │  │  │           │  └─ name: amountOut
      │  │  │           └─ right
      │  │  │              ├─ type: BinaryOperation
      │  │  │              ├─ operator: /
      │  │  │              ├─ left
      │  │  │              │  ├─ type: Identifier
      │  │  │              │  └─ name: numerator
      │  │  │              └─ right
      │  │  │                 ├─ type: Identifier
      │  │  │                 └─ name: denominator
      │  │  ├─ visibility: internal
      │  │  ├─ modifiers
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability: pure
      │  ├─ 24
      │  │  ├─ type: FunctionDefinition
      │  │  ├─ name: getAmountsOut
      │  │  ├─ parameters
      │  │  │  ├─ 0
      │  │  │  │  ├─ type: VariableDeclaration
      │  │  │  │  ├─ typeName
      │  │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │  │  │  └─ name: uint
      │  │  │  │  ├─ name: amountIn
      │  │  │  │  ├─ storageLocation
      │  │  │  │  ├─ isStateVar: false
      │  │  │  │  └─ isIndexed: false
      │  │  │  └─ 1
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ArrayTypeName
      │  │  │     │  ├─ baseTypeName
      │  │  │     │  │  ├─ type: ElementaryTypeName
      │  │  │     │  │  └─ name: address
      │  │  │     │  └─ length
      │  │  │     ├─ name: path
      │  │  │     ├─ storageLocation: memory
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ returnParameters
      │  │  │  └─ 0
      │  │  │     ├─ type: VariableDeclaration
      │  │  │     ├─ typeName
      │  │  │     │  ├─ type: ArrayTypeName
      │  │  │     │  ├─ baseTypeName
      │  │  │     │  │  ├─ type: ElementaryTypeName
      │  │  │     │  │  └─ name: uint
      │  │  │     │  └─ length
      │  │  │     ├─ name: amounts
      │  │  │     ├─ storageLocation: memory
      │  │  │     ├─ isStateVar: false
      │  │  │     └─ isIndexed: false
      │  │  ├─ body
      │  │  │  ├─ type: Block
      │  │  │  └─ statements
      │  │  │     ├─ 0
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: FunctionCall
      │  │  │     │     ├─ expression
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: require
      │  │  │     │     ├─ arguments
      │  │  │     │     │  ├─ 0
      │  │  │     │     │  │  ├─ type: BinaryOperation
      │  │  │     │     │  │  ├─ operator: >=
      │  │  │     │     │  │  ├─ left
      │  │  │     │     │  │  │  ├─ type: MemberAccess
      │  │  │     │     │  │  │  ├─ expression
      │  │  │     │     │  │  │  │  ├─ type: Identifier
      │  │  │     │     │  │  │  │  └─ name: path
      │  │  │     │     │  │  │  └─ memberName: length
      │  │  │     │     │  │  └─ right
      │  │  │     │     │  │     ├─ type: NumberLiteral
      │  │  │     │     │  │     ├─ number: 2
      │  │  │     │     │  │     └─ subdenomination
      │  │  │     │     │  └─ 1
      │  │  │     │     │     ├─ type: StringLiteral
      │  │  │     │     │     ├─ value: APM: INVALID_PATH
      │  │  │     │     │     └─ parts
      │  │  │     │     │        └─ 0: APM: INVALID_PATH
      │  │  │     │     └─ names
      │  │  │     ├─ 1
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: Identifier
      │  │  │     │     │  └─ name: amounts
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: FunctionCall
      │  │  │     │        ├─ expression
      │  │  │     │        │  ├─ type: NewExpression
      │  │  │     │        │  └─ typeName
      │  │  │     │        │     ├─ type: ArrayTypeName
      │  │  │     │        │     ├─ baseTypeName
      │  │  │     │        │     │  ├─ type: ElementaryTypeName
      │  │  │     │        │     │  └─ name: uint
      │  │  │     │        │     └─ length
      │  │  │     │        ├─ arguments
      │  │  │     │        │  └─ 0
      │  │  │     │        │     ├─ type: MemberAccess
      │  │  │     │        │     ├─ expression
      │  │  │     │        │     │  ├─ type: Identifier
      │  │  │     │        │     │  └─ name: path
      │  │  │     │        │     └─ memberName: length
      │  │  │     │        └─ names
      │  │  │     ├─ 2
      │  │  │     │  ├─ type: ExpressionStatement
      │  │  │     │  └─ expression
      │  │  │     │     ├─ type: BinaryOperation
      │  │  │     │     ├─ operator: =
      │  │  │     │     ├─ left
      │  │  │     │     │  ├─ type: IndexAccess
      │  │  │     │     │  ├─ base
      │  │  │     │     │  │  ├─ type: Identifier
      │  │  │     │     │  │  └─ name: amounts
      │  │  │     │     │  └─ index
      │  │  │     │     │     ├─ type: NumberLiteral
      │  │  │     │     │     ├─ number: 0
      │  │  │     │     │     └─ subdenomination
      │  │  │     │     └─ right
      │  │  │     │        ├─ type: Identifier
      │  │  │     │        └─ name: amountIn
      │  │  │     └─ 3
      │  │  │        ├─ type: ForStatement
      │  │  │        ├─ initExpression
      │  │  │        │  ├─ type: VariableDeclarationStatement
      │  │  │        │  ├─ variables
      │  │  │        │  │  └─ 0
      │  │  │        │  │     ├─ type: VariableDeclaration
      │  │  │        │  │     ├─ typeName
      │  │  │        │  │     │  ├─ type: ElementaryTypeName
      │  │  │        │  │     │  └─ name: uint
      │  │  │        │  │     ├─ name: i
      │  │  │        │  │     ├─ storageLocation
      │  │  │        │  │     ├─ isStateVar: false
      │  │  │        │  │     └─ isIndexed: false
      │  │  │        │  └─ initialValue
      │  │  │        ├─ conditionExpression
      │  │  │        │  ├─ type: BinaryOperation
      │  │  │        │  ├─ operator: <
      │  │  │        │  ├─ left
      │  │  │        │  │  ├─ type: Identifier
      │  │  │        │  │  └─ name: i
      │  │  │        │  └─ right
      │  │  │        │     ├─ type: BinaryOperation
      │  │  │        │     ├─ operator: -
      │  │  │        │     ├─ left
      │  │  │        │     │  ├─ type: MemberAccess
      │  │  │        │     │  ├─ expression
      │  │  │        │     │  │  ├─ type: Identifier
      │  │  │        │     │  │  └─ name: path
      │  │  │        │     │  └─ memberName: length
      │  │  │        │     └─ right
      │  │  │        │        ├─ type: NumberLiteral
      │  │  │        │        ├─ number: 1
      │  │  │        │        └─ subdenomination
      │  │  │        ├─ loopExpression
      │  │  │        │  ├─ type: ExpressionStatement
      │  │  │        │  └─ expression
      │  │  │        │     ├─ type: UnaryOperation
      │  │  │        │     ├─ operator: ++
      │  │  │        │     ├─ subExpression
      │  │  │        │     │  ├─ type: Identifier
      │  │  │        │     │  └─ name: i
      │  │  │        │     └─ isPrefix: false
      │  │  │        └─ body
      │  │  │           ├─ type: Block
      │  │  │           └─ statements
      │  │  │              ├─ 0
      │  │  │              │  ├─ type: VariableDeclarationStatement
      │  │  │              │  ├─ variables
      │  │  │              │  │  ├─ 0
      │  │  │              │  │  │  ├─ type: VariableDeclaration
      │  │  │              │  │  │  ├─ name: reserveIn
      │  │  │              │  │  │  ├─ typeName
      │  │  │              │  │  │  │  ├─ type: ElementaryTypeName
      │  │  │              │  │  │  │  └─ name: uint
      │  │  │              │  │  │  ├─ storageLocation
      │  │  │              │  │  │  ├─ isStateVar: false
      │  │  │              │  │  │  └─ isIndexed: false
      │  │  │              │  │  └─ 1
      │  │  │              │  │     ├─ type: VariableDeclaration
      │  │  │              │  │     ├─ name: reserveOut
      │  │  │              │  │     ├─ typeName
      │  │  │              │  │     │  ├─ type: ElementaryTypeName
      │  │  │              │  │     │  └─ name: uint
      │  │  │              │  │     ├─ storageLocation
      │  │  │              │  │     ├─ isStateVar: false
      │  │  │              │  │     └─ isIndexed: false
      │  │  │              │  └─ initialValue
      │  │  │              │     ├─ type: FunctionCall
      │  │  │              │     ├─ expression
      │  │  │              │     │  ├─ type: Identifier
      │  │  │              │     │  └─ name: getReserves
      │  │  │              │     ├─ arguments
      │  │  │              │     │  ├─ 0
      │  │  │              │     │  │  ├─ type: IndexAccess
      │  │  │              │     │  │  ├─ base
      │  │  │              │     │  │  │  ├─ type: Identifier
      │  │  │              │     │  │  │  └─ name: path
      │  │  │              │     │  │  └─ index
      │  │  │              │     │  │     ├─ type: Identifier
      │  │  │              │     │  │     └─ name: i
      │  │  │              │     │  └─ 1
      │  │  │              │     │     ├─ type: IndexAccess
      │  │  │              │     │     ├─ base
      │  │  │              │     │     │  ├─ type: Identifier
      │  │  │              │     │     │  └─ name: path
      │  │  │              │     │     └─ index
      │  │  │              │     │        ├─ type: BinaryOperation
      │  │  │              │     │        ├─ operator: +
      │  │  │              │     │        ├─ left
      │  │  │              │     │        │  ├─ type: Identifier
      │  │  │              │     │        │  └─ name: i
      │  │  │              │     │        └─ right
      │  │  │              │     │           ├─ type: NumberLiteral
      │  │  │              │     │           ├─ number: 1
      │  │  │              │     │           └─ subdenomination
      │  │  │              │     └─ names
      │  │  │              └─ 1
      │  │  │                 ├─ type: ExpressionStatement
      │  │  │                 └─ expression
      │  │  │                    ├─ type: BinaryOperation
      │  │  │                    ├─ operator: =
      │  │  │                    ├─ left
      │  │  │                    │  ├─ type: IndexAccess
      │  │  │                    │  ├─ base
      │  │  │                    │  │  ├─ type: Identifier
      │  │  │                    │  │  └─ name: amounts
      │  │  │                    │  └─ index
      │  │  │                    │     ├─ type: BinaryOperation
      │  │  │                    │     ├─ operator: +
      │  │  │                    │     ├─ left
      │  │  │                    │     │  ├─ type: Identifier
      │  │  │                    │     │  └─ name: i
      │  │  │                    │     └─ right
      │  │  │                    │        ├─ type: NumberLiteral
      │  │  │                    │        ├─ number: 1
      │  │  │                    │        └─ subdenomination
      │  │  │                    └─ right
      │  │  │                       ├─ type: FunctionCall
      │  │  │                       ├─ expression
      │  │  │                       │  ├─ type: Identifier
      │  │  │                       │  └─ name: getAmountOut
      │  │  │                       ├─ arguments
      │  │  │                       │  ├─ 0
      │  │  │                       │  │  ├─ type: IndexAccess
      │  │  │                       │  │  ├─ base
      │  │  │                       │  │  │  ├─ type: Identifier
      │  │  │                       │  │  │  └─ name: amounts
      │  │  │                       │  │  └─ index
      │  │  │                       │  │     ├─ type: Identifier
      │  │  │                       │  │     └─ name: i
      │  │  │                       │  ├─ 1
      │  │  │                       │  │  ├─ type: Identifier
      │  │  │                       │  │  └─ name: reserveIn
      │  │  │                       │  └─ 2
      │  │  │                       │     ├─ type: Identifier
      │  │  │                       │     └─ name: reserveOut
      │  │  │                       └─ names
      │  │  ├─ visibility: external
      │  │  ├─ modifiers
      │  │  ├─ override
      │  │  ├─ isConstructor: false
      │  │  ├─ isReceiveEther: false
      │  │  ├─ isFallback: false
      │  │  ├─ isVirtual: false
      │  │  └─ stateMutability: view
      │  └─ 25
      │     ├─ type: FunctionDefinition
      │     ├─ name: removeLiquidity
      │     ├─ parameters
      │     │  ├─ 0
      │     │  │  ├─ type: VariableDeclaration
      │     │  │  ├─ typeName
      │     │  │  │  ├─ type: ElementaryTypeName
      │     │  │  │  └─ name: address
      │     │  │  ├─ name: _to
      │     │  │  ├─ storageLocation
      │     │  │  ├─ isStateVar: false
      │     │  │  └─ isIndexed: false
      │     │  ├─ 1
      │     │  │  ├─ type: VariableDeclaration
      │     │  │  ├─ typeName
      │     │  │  │  ├─ type: ElementaryTypeName
      │     │  │  │  └─ name: address
      │     │  │  ├─ name: tokenAddress
      │     │  │  ├─ storageLocation
      │     │  │  ├─ isStateVar: false
      │     │  │  └─ isIndexed: false
      │     │  └─ 2
      │     │     ├─ type: VariableDeclaration
      │     │     ├─ typeName
      │     │     │  ├─ type: ElementaryTypeName
      │     │     │  └─ name: uint
      │     │     ├─ name: amount
      │     │     ├─ storageLocation
      │     │     ├─ isStateVar: false
      │     │     └─ isIndexed: false
      │     ├─ returnParameters
      │     ├─ body
      │     │  ├─ type: Block
      │     │  └─ statements
      │     │     ├─ 0
      │     │     │  ├─ type: ExpressionStatement
      │     │     │  └─ expression
      │     │     │     ├─ type: FunctionCall
      │     │     │     ├─ expression
      │     │     │     │  ├─ type: MemberAccess
      │     │     │     │  ├─ expression
      │     │     │     │  │  ├─ type: FunctionCall
      │     │     │     │  │  ├─ expression
      │     │     │     │  │  │  ├─ type: Identifier
      │     │     │     │  │  │  └─ name: IERC20
      │     │     │     │  │  ├─ arguments
      │     │     │     │  │  │  └─ 0
      │     │     │     │  │  │     ├─ type: Identifier
      │     │     │     │  │  │     └─ name: tokenAddress
      │     │     │     │  │  └─ names
      │     │     │     │  └─ memberName: safeTransfer
      │     │     │     ├─ arguments
      │     │     │     │  ├─ 0
      │     │     │     │  │  ├─ type: Identifier
      │     │     │     │  │  └─ name: _to
      │     │     │     │  └─ 1
      │     │     │     │     ├─ type: Identifier
      │     │     │     │     └─ name: amount
      │     │     │     └─ names
      │     │     └─ 1
      │     │        ├─ type: ExpressionStatement
      │     │        └─ expression
      │     │           ├─ type: FunctionCall
      │     │           ├─ expression
      │     │           │  ├─ type: Identifier
      │     │           │  └─ name: updateWhenRemoveLiquidity
      │     │           ├─ arguments
      │     │           │  ├─ 0
      │     │           │  │  ├─ type: Identifier
      │     │           │  │  └─ name: amount
      │     │           │  └─ 1
      │     │           │     ├─ type: Identifier
      │     │           │     └─ name: tokenAddress
      │     │           └─ names
      │     ├─ visibility: external
      │     ├─ modifiers
      │     │  └─ 0
      │     │     ├─ type: ModifierInvocation
      │     │     ├─ name: onlyBank
      │     │     └─ arguments
      │     ├─ override
      │     ├─ isConstructor: false
      │     ├─ isReceiveEther: false
      │     ├─ isFallback: false
      │     ├─ isVirtual: false
      │     └─ stateMutability
      └─ kind: contract

