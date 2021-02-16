SOLIDITY ETHEREUM CONTRACT 
What is Solidity?
Solidity is an object-oriented programming language for writing smart contracts. It is used for implementing smart contracts on various blockchain platforms, most notably, Ethereum.
It is a very basic contract that will give a better understanding on how ethereum contract works.
Okay, So let's start off by going to remix.ethereum.org
What is Remix-Ethereum IDE?
Remix is basicaly an open source web and destop application that allows developing, deploying and administering smart contracts for Ethereum.
So we write the ethereum contracts in .sol files that is just an abbrevation for solidity
Solity majorly works on the data structure contracts. Contracts can be seen as very similar to classes in other object oriented programming languages.
We can define methods(functions) and variables inside the smart contract.

CODE WALK THROUGH
pragma solidity ^0.4.17; // This line indicates the version of Solidity we are writing our code in 
contract Inbox{
    string public message;
     
     function Inbox(string imess) public{
         message=imess;
     }
    
    function setMessage(string newmess) public{
        message= newmess;
    }
    
    function getMessage() public view returns(string){
        return message;
    }
}
