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

## Avanced Smart Contracts

### Basic types in Solidity

* String: sequence of characters.
* Bool: Boolean value.
* Int: Integer.
* Uint: 'Unsigned' integer.
* Fixed/ ufixed: 'Fixed' point number.
* Address: Has methods tied to it for sending money.

### Referenced types
* Fixed array. Array that contains a single type of element. Has an unchanging length.
* Dynamic array. Array that contains a single type of element. Can change in size over time.
* Mapping. Collection of key value pairs. All keys must be of the same type, and all values must be of the same type.
* Struct. Collection of key values pairs that can have different types.

### The message global variable

There is a message global variable in any call or transaction with the following properties:
* *msg.data*. 'Data' field from the call or transaction that invoked the current function.
* *msg.gas*. Amount of gas the current function invocation has available.
* *msg.sender*. Address of the account that started the current function invocation.
* *msg.value*. Amount of ether (in wei) that was sent along with the function invocation.
