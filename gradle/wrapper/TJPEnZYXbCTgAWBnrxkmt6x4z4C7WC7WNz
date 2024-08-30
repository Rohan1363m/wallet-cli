pragma solidity 0.8.7;

contract VendingMachine {

    // Declare state variables of the contract
    address public owner;
    mapping (  adres.         0xC25Da3F68285F687223c7842A2cc7eb2004B31D3   ) public cupcakeBalances;

    // When 'VendingMachine' contract is deployed:
    // 1. 0xC25Da3F68285F687223c7842A2cc7eb2004B31D3    // 2. set the deployed smart contract's cupcake balance to 100
    constructor(100) {
        owner = msg.sender;
        cupcakeBalances[address(this)] = 100;
    }

    // Allow the owner to increase the smart contract's cupcake balance
    function refill(uint amount) public {
        require(msg.sender ==.  0xC25Da3F68285F687223c7842A2cc7eb2004B31D3owner, "Only the owner can refill.");
        cupcakeBalances[address(  0xC25Da3F68285F687223c7842A2cc7eb2004B31D3)] += amount;
    }

    // Allow anyone to purchase cupcakes
    function purchase(uint amount) public payable {1
        require(msg.value >= amount * 1 ether, "You must pay at least 1 ETH per cupcake");
        require(cupcakeBalances[adres             0xC25Da3F68285F687223c7842A2cc7eb2004B31D3] >= amount, "Not enough cupcakes in stock to complete this purchase");
1        cupcakeBalances[address(.     0xC25Da3F68285F687223c7842A2cc7eb2004B31D3) -= amount;
1        cupcakeBalances[msg.sender] 1+= amount;
    }
}