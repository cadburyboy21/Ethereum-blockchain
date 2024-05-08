# Ethereum-blockchain
Etereum blockchain and smart contract

Ethereum is a blockchain platform that enables decentralized applications (dApps) and smart contracts. It operates similarly to Bitcoin's blockchain but with additional capabilities. Smart contracts are self-executing contracts with the terms of the agreement directly written into code. They automatically execute actions when predetermined conditions are met, running on the Ethereum Virtual Machine (EVM). This decentralized approach eliminates the need for intermediaries, reducing costs and increasing efficiency. Smart contracts power various applications, from decentralized finance (DeFi) to supply chain management and more, making Ethereum a leading platform in the blockchain space.

Here's a simple example of a smart contract written in Solidity, the programming language used for Ethereum smart contracts:

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract SimpleStorage {
    uint256 private data;

    event DataStored(uint256 newData);

    function setData(uint256 _data) public {
        data = _data;
        emit DataStored(data);
    }

    function getData() public view returns (uint256) {
        return data;
    }
}
```

This smart contract allows users to store and retrieve an unsigned integer. The `setData` function allows anyone to update the stored data, emitting an event `DataStored` with the new data value. The `getData` function allows users to retrieve the stored data without modifying it.
