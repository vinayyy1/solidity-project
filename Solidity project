// SPDX-License-Identifier: MIT
pragma solidity 0.8.18;

contract UniqueToken {

    // Public variables to store details about the coin
    string public tokenName = "UniqueToken";
    string public tokenSymbol = "UTK";
    uint256 public tokenTotalSupply;

    // Mapping of addresses to balances
    mapping(address => uint256) public tokenBalances;

    // Mint function to create new tokens
    function mintTokens(address recipient, uint256 amount) public {
        tokenTotalSupply += amount;
        tokenBalances[recipient] += amount;
    }

    // Burn function to destroy tokens
    function burnTokens(address holder, uint256 amount) public {
        require(tokenBalances[holder] >= amount, "Insufficient balance to burn");
        tokenTotalSupply -= amount;
        tokenBalances[holder] -= amount;
    }
}
ChatGPT
ChatGPT
