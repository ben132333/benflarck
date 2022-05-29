# Solidity project: create an ERC20 Token 

I created an ERC-20 token, called Benflarck (BFL), and deployed it to the Rinkeby testnet.

It's most remarkable feature is that it's completely useless because I own 100% of the BFL supply and don't have a distribution or supply mechanism in mind. It's still a usefull first project because you pick an IDE to work in, learn to test Solidity code on a locally hosted node and deploy a smart contract to a public testnet.

The solidity code is available on the OpenZeppelin:
https://docs.openzeppelin.com/contracts/4.x/erc20a

OpenZepplin has a guide to set up your first smart contract (creating the project, testing, and deploying it):
https://docs.openzeppelin.com/learn/

## secret.js

If you'd want to deploy your own contract, you'd need to create a secret.json, containing:

{
    "mnemonic": "your mnemonic bla bla bla ...",
    "alchemyApiKey": "something_something_..."
}

Benflarck
Contract address: https://rinkeby.etherscan.io/token/0x2A05555379daC92862BAC9dDe8a704cD69FDa477

## Connecting to the contract via CLI:

> npx hardhat console --network rinkeby

> const Benflarck = await ethers.getContractFactory('Benflarck');

> const benflarck = await Benflarck.attach('0x0017f2F644E842f3cf3F8E408dA38F900006394f');

> await benflarck.balanceOf("0xC5aBed2f8dB85c850802C8F11AD066fFEe17706B")


