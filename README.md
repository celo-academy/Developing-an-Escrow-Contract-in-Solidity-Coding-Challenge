## Introduction

Solidity is a high-level programming language used for writing smart contracts on blockchain platforms like Celo. Smart contracts can be used to automate complex transactions and agreements, such as an escrow system. In this challenge, you will construct a simple escrow contract using Solidity.

## Problem Statement

Design a smart contract that simulates an escrow agreement with the following requirements:

1. The contract should allow a buyer to initiate an escrow transaction by specifying the seller's address and the agreed amount.
2. The contract should hold the funds until the buyer confirms that they have received the goods or services.
3. The contract should allow the buyer to release the funds to the seller once the goods or services have been received.
4. If the buyer is not satisfied, the contract should have a dispute resolution mechanism where a third-party escrow agent can arbitrate and decide where the funds should go.
5. The contract should prevent the buyer from initiating a new escrow transaction if the previous one is not resolved.

## Hints

- Use Solidity's `address payable` data type to handle addresses that can receive funds.
- Use `msg.sender` and `msg.value` to get the sender's address and the sent amount.
- Implement `modifier` functions to enforce that only the appropriate parties can call certain functions.
- Use `enum` to represent the state of the escrow.

## Evaluation Criteria

- **Correctness**: The contract should compile without errors and meet all requirements.
- **Readability**: The contract should be well-documented, with comments explaining the code.
- **Testability**: You should provide examples of how to test each function of the contract.

Please note that real-world escrow contracts would need more security measures and edge case handling than this simple exercise provides.

For a comprehensive understanding of Celo smart contracts and Solidity, please refer to the Celo and Solidity tutorials.

## Submission

Please provide a link to your PR on GitHub, including your escrow contract. Also include any notes or comments you think are necessary for understanding your solution. Lastly, provide a brief explanation about how each function of the contract should be tested.
