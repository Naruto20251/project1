
# MyToken Solidity Contract

This is a simple Solidity smart contract for a custom token called MyToken. It implements basic functionality for creating and managing tokens.

## Requirements

1. The contract has public variables to store the details of the coin: Token Name, Token Abbreviation, and Total Supply.
2. It includes a mapping of addresses to balances (`mapping(address => uint) public balances`).
3. The contract contains a `mint` function to increase the total supply and the balance of the sender's address.
4. It also features a `burn` function to destroy tokens, reducing both the total supply and the sender's balance.
5. The `burn` function includes conditionals to ensure the sender's balance is sufficient for burning.

## Contract Details

- Token Name: abcc
- Token Abbreviation: AB
- Total Supply: 100

## Functions

### `mint(address add, uint val)`

This function increases the balance of the specified address by the given value and adds the same value to the total supply.

#### Parameters

- `add` (address): The address to which the tokens will be minted.
- `val` (uint): The amount of tokens to mint.

### `burn(address add, uint val)`

This function reduces the balance of the specified address by the given value and deducts the same value from the total supply, provided that the sender's balance is greater than or equal to the specified value.

#### Parameters

- `add` (address): The address from which the tokens will be burned.
- `val` (uint): The amount of tokens to burn.

## Usage

1. Deploy the `MyToken` contract to a compatible Ethereum Virtual Machine (EVM) using Solidity version 0.8.18.
2. Interact with the contract functions to mint and burn tokens.
3. Ensure that the conditions for burning tokens (sufficient sender balance) are met before invoking the `burn` function.

## Note

This contract is provided as a basic example and should be thoroughly reviewed, tested, and adapted before deploying to any production environment.

## License

This contract is licensed under the MIT License.

