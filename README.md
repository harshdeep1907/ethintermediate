# ethintermediate

This is a Solidity smart contract that demonstrates different error handling techniques using `assert`, `revert`, and `require` functions.

## License

This contract is using the MIT License.

## Prerequisites

- Solidity ^0.8.17

## Contract Details

The `ErrorHandling` contract provides the following functions:

### `testAssert(uint number)`

- This function demonstrates the usage of the `assert` function.
- It takes a `number` parameter and checks if it is not equal to zero using the `assert` statement.
- If the condition fails, it triggers an "Internal error" and aborts the execution.

### `divide(uint _numerator, uint _denominator)`

- This function demonstrates the usage of the `revert` function.
- It takes `_numerator` and `_denominator` parameters and performs division.
- If the `_numerator` is less than `_denominator`, it reverts the transaction with a custom error message stating that Please provide a numerator greater than the denominato.
- If the condition is met, it returns the result of the division.

### `multiply(uint input)`

- This function demonstrates the usage of the `require` function.
- It takes an `input` parameter and performs multiplication with a predefined constant `variableB`.
- It first checks if `input` is greater than zero using the `require` statement.
- If the condition fails, it reverts the transaction with a custom error message stating that the value of `a` should not be zero.
- If the condition is met, it returns the result of the multiplication.

## Usage

1. Make sure you have Solidity ^0.8.17 installed.
2. Compile and deploy the `ErrorHandling` contract to a supported Ethereum network.
3. Interact with the deployed contract by calling the available functions and providing the required parameters.

## Video Walkthrough

- https://www.loom.com/share/a5754cdeff374665b643d9292e9e9fa3?sid=e4afa845-e081-4b7b-84c9-46c8e9785dc6

Feel free to explore and modify the contract according to your needs!
