*Solidity Token Readme*

### INTRODUCTION
This readme provides an overview of a Solidity smart contract that implements a custom token called "Dotless" (symbol: dtls). The contract includes functionalities for minting and burning tokens, as well as storing token details such as name, abbreviation, and total supply.

### CONTRACT DETAILS
#### Public Variables
- 'token_Name': Stores the name of the token ("Dotless").
- 'token_Abbrv': Stores the abbreviation of the token ("dtls").
- 'TotalSupply': Stores the total supply of the token. Initialized to 0 and updated dynamically.

#### Mapping
- 'balances': A mapping of addresses to token balances. Keeps track of the balance of each address.

#### Mint Function
- 'mint(address _address, uint _value) public': Increases the total supply by the specified value and increases the balance of the specified address by that amount.

#### Burn Function
- 'burn(address _address, uint _value) public': Decreases the total supply by the specified value and decreases the balance of the specified address by that amount. Includes conditionals to ensure the balance of the sender is sufficient to burn the specified amount.

### REQUIREMENTS
The contract fulfills the following requirements:
1. Public variables store details about the coin (token name, abbreviation, total supply).
2. A mapping of addresses to balances is implemented.
3. The mint function increases the total supply and the balance of the sender address.
4. The burn function decreases the total supply and the balance of the sender address, with conditionals to ensure balance sufficiency.

### CONCLUSION
With this Solidity smart contract, you can create and manage custom tokens on the Ethereum blockchain. The contract provides flexibility for minting new tokens and burning existing ones, while also maintaining transparency with public variables and mappings.
