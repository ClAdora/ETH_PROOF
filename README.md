# MyToken Solidity Contract

## Introduction

The MyToken Solidity contract is a simple example that demonstrates the basic features of a token smart contract written in Solidity. This contract includes functionalities for minting and burning tokens and tracks token balances for different addresses. It serves as a starting point for learning how to create and interact with Ethereum smart contracts.

## Getting Started

To work with the MyToken contract, you can follow these steps:

1. Clone this repository to your local machine or use Remix, an online Solidity IDE.

2. If using Remix:
   - Go to the Remix website at [https://remix.ethereum.org/](https://remix.ethereum.org/).
   - Create a new file with a `.sol` extension (e.g., `MyToken.sol`).
   - Copy and paste the content of the `MyToken.sol` contract into the file.

3. Compile the contract:
   - In Remix, go to the "Solidity Compiler" tab.
   - Set the "Compiler" version to `0.8.18` (or another compatible version).
   - Click the "Compile MyToken.sol" button.

4. Deploy the contract:
   - In Remix, go to the "Deploy & Run Transactions" tab.
   - Select the "MyToken" contract from the dropdown menu.
   - Click the "Deploy" button.

5. Interact with the contract:
   - You can now interact with the deployed contract using the provided functions, such as `mint` and `burn`.

## Contract Details

### Public Variables

- `tokenName`: The name of the token (e.g., "Clintt").
- `tokenAbbrv`: The token abbreviation (e.g., "Adora").
- `totalSupply`: The total supply of tokens.

### Functions

- `mint(address _address, uint _value)`: Mint new tokens and increase the balance of an address.
- `burn(address _address, uint _value)`: Burn tokens and decrease the balance of an address, with validation to ensure the address has sufficient tokens.

## Examples

Here are some examples of how to use the contract functions:

**Minting Tokens:**

```javascript
// Mint 100 tokens to an address
myToken.mint("0xAddressHere", 100);
