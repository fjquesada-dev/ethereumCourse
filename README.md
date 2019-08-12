# Ethereum Course

## Smart Contracts with Solidity
### Ganache
Local test network:
* Generate some number of address accounts.
* It is possible to send transactions to this network.
* It can be deployed contracts to this network.
* Transactions are completed almost instantaneously.

### Web3

Connecting Javascript with Ethereum

* Web3 needs a provider to connect to a blockchain network

#### Contracts

* *Interact with deployed contract*
  * Need ABI and address of deployed contract.
* *Create a new contract*
  * Need ABI and Bytecode.

### Mocha
Testing Javascript applications (General purpose testing framework)

#### Functions

* it -> Run a test and make an assertion. One individual assertion.
* describe -> Groups together a collection of 'it' functions.
* beforeEach -> Execute some general setup code.

#### Structure

We are going to use Mocha as follows:

* Deploy a new contract *beforeEach*
* Manipulate the contract *it*
* Make an asserting about the contract *it*
