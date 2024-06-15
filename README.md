# My Token

This is a Solidity program that provides the functionality of minting and burning a token, somewhat. It does this by keeping track of the supply of a token and the particular balance of an address. This is my submission for the ETH Proof: Solidity Beginner's course.

## Description

It is a program written in Solidity. It only has one main functionality: minting and burning tokens.

This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract has a single function that returns the string "Hello World!". This program serves as a simple and straightforward introduction to Solidity programming, and can be used as a stepping stone for more complex projects in the future.

### Program Functions

```javascript

    // mint function
    function mint (address _address, uint _value) public {
        totalSupply += _value;
        balances[_address] += _value;
    }

    // burn function
    function burn (address _address, uint _value) public {
        if (balances[_address] >= _value) {
            totalSupply -= _value;
            balances[_address] -= _value;
        }

```

The mint function takes an address and a value represented by an unsigned integer. That value is the amount of tokens to amount.

The burn function also takes both an address and value, however the value is the amount of tokens to burn.

Both of these functions modify the balance of an address.

## Authors

Andre A. Aquino 

