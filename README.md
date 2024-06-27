# SimpleContract

## Overview

This Solidity smart contract, `SimpleContract`, demonstrates basic state management by initializing a `data` variable with a value provided during deployment. It includes functions to update `data` (`setData`) and retrieve its current value (`getData`). This contract serves as a fundamental example for beginners learning Solidity.

## Description

The `SimpleContract` is a basic smart contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. It includes:
- A state variable `data` of type `uint256` to store an integer value.
- Two functions:
  - `setData(uint256 _data)`: Allows setting the value of `data`.
  - `getData()`: Returns the current value of `data`.

This contract demonstrates essential concepts like state variables, function visibility (`public` and `view`), and function modifiers (`pure` and `view`).

## Getting Started

### Executing Program

To interact with this contract, follow these steps using Remix, an online Solidity IDE:

1. **Access Remix:**
   - Go to [Remix IDE](https://remix.ethereum.org/).

2. **Create and Save File:**
   - Click on the "+" icon in the left-hand sidebar to create a new file.
   - Save the file with a .sol extension (e.g., `SimpleContract.sol`).

3. **Code:**
   - Write the provided Solidity code into the file:

     ```solidity
     // SPDX-License-Identifier: MIT
     pragma solidity ^0.8.0;

     contract SimpleContract {
         uint256 public data;

         function setData(uint256 _data) public {
             data = _data;
         }

         function getData() public view returns (uint256) {
             return data;
         }
     }
     ```

4. **Compile Code:**
   - Switch to the "Solidity Compiler" tab in Remix.
   - Set the "Compiler" option to "0.8.0" (or another compatible version).
   - Click on "Compile SimpleContract.sol" to compile the contract.

5. **Deploy Contract:**
   - Navigate to the "Deploy & Run Transactions" tab in Remix.
   - Select the "SimpleContract" contract from the dropdown menu.
   - Click on the "Deploy" button to deploy the contract.

6. **Interact with Contract:**
   - Once deployed, interact with the contract:
     - Use the `setData` function to set a new value for `data`.
     - Use the `getData` function to retrieve the current value of `data`.

## Authors

- Ambesh Dubey

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
