#  A Simple DeFI Kingdom Clone

## Description

This project is a basic clone of blockchain based game. In this project, players can collect, build and battle with their digital assets which is done over custom EVM subnet on Avalanche.

## Getting Started

### Executing program

To run this project, follow these steps:

1. Download [Oracle VM VirtualBox](https://www.virtualbox.org/). Install and configure it.
2. Now download any Microsoft Windows Subsystem for Linux (WSL) like [Ubuntu](https://ubuntu.com/desktop/wsl) or [Parrot](https://parrotsec.org/download/). Install and configure it on VirtualBox.
3. After opening the WSL, open its terminal and install Avalanche-CLI. [ You can find installation instructions for the Avalanche CLI in the official documentation](https://docs.avax.network/tooling/cli-guides/install-avalanche-cli).
4. Once you have the Avalanche CLI installed, you can create a new subnet by running the command avalanche subnet create mySubnet in your terminal. This will create a new subnet with the name "mySubnet" on your local machine.
5. When creating a new subnet, you will be prompted to select a subnet type. Choose the SubnetEVM option to create an EVM Subnet on your local machine and follow the steps in step 6.
6. avalanche subnet create mySubnet <br>
Attempted to check if a new version is available, but couldn't find the currently running version information <br>
Make sure to follow official instructions, or automatic updates won't be available for you <br>
✔ Subnet-EVM <br>
creating subnet mySubnet <br>
Enter your subnet's ChainId. It can be any positive integer. <br>
ChainId: 5648 <br>
Select a symbol for your subnet's native token <br>
Token symbol: SK <br>
✔ Use latest version <br>
✔ Low disk use    / Low Throughput    1.5 mil gas/s (C-Chain's setting) <br>
✔ Airdrop 1 million tokens to the default address (do not use in production) <br>
✔ No <br>
7. After selecting the EVM Subnet option, you can deploy the subnet by running the command avalanche subnet deploy mySubnet and selecting to deploy your subnet on your local network. This will deploy your new EVM Subnet on your local machine.
8. Once your EVM Subnet is deployed, the console will display all the details about the subnet you just created.
9. Create a local network on your wallet using the subnet details.
10. Now, got to [Remix IDE](https://remix.ethereum.org/#lang=en&optimize=false&runs=200&evmVersion=null&version=soljson-v0.8.26+commit.8a97fa7a.js) and create two files of name `ERC20.sol` and `vault.sol` Copy paste the code.
11. Now, compile both the contracts under Compiler tab.
12. Now, connect Remix with the MetaMask wallet using Injected Provider.
13. First deploy `ERC20.sol` contract and then copy the contract's address and by using the address, deploy `vault.sol` contract.
14. After deploying the contracts, you can interact with the contract by calling its functions through the Remix interface.
15. You can mint tokens, can approve the transactions done by vault contract, deposit and withdraw using vault contract. 

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Authors

Srijan Kumar  
[@Srijan](srijankumar11627@gmail.com)
