# EmployeeStorage

Employee data storage system with gas-optimized storage packing and share management functionality.

## Description

This contract demonstrates efficient storage packing techniques in Solidity to minimize gas costs. It manages employee information including shares, salary, name, and ID number with proper validation and error handling.

## Features

- **Storage Optimization**: Variables packed to minimize storage slots
- **Share Management**: Grant shares with validation (max 5,000 total)
- **Custom Errors**: Efficient error handling with custom error types
- **Assembly Integration**: Low-level storage inspection functionality

## Deployment Instructions

1. Open [Remix IDE](https://remix.ethereum.org/)
2. Create a new file and copy-paste the contract code
3. Compile the contract using Solidity ^0.8.0
4. Deploy on **Base Sepolia Testnet** with constructor parameters:
   - **shares**: `1000`
   - **name**: `"Pat"`
   - **salary**: `50000`
   - **idNumber**: `112358132134`
5. Interact with the functions:
   - `viewSalary()` - View employee salary
   - `viewShares()` - View employee shares
   - `grantShares(uint16 _newShares)` - Grant additional shares
   - `checkForPacking(uint _slot)` - Inspect storage packing

## Submit Exercise

[📖 Submit Storage Exercise](https://docs.base.org/learn/storage/storage-exercise)
