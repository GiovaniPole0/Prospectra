// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract SimpleERC20 {
    string public name = "Prospectra";
    string public symbol = "SPEC";
    uint8 public decimals = 18;
    uint256 public totalSupply;
    mapping(address => uint256) public balanceOf;

event Transfer(address indexed from, address indexed to, uint256 value);

constructor(uint256 initialSupply) {
        totalSupply = initialSupply * (10 ** uint256(decimals));
        balanceOf[msg.sender] = totalSupply;
        emit Transfer(address(0), msg.sender, totalSupply);
    }

function transfer(address to, uint256 value) external returns (bool) {
        require(to != address(0), "Transfer to the zero address");
        require(balanceOf[msg.sender] >= value, "Insufficient balance");

balanceOf[msg.sender] -= value;
        balanceOf[to] += value;
        emit Transfer(msg.sender, to, value);
        return true;
    }
}
