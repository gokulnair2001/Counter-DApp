# Counter
This repo is for beginners who want to have a hands-on with Dapp(Decentralised applications). Basically in this repo, I have deployed a Smart Contract on **Ethereum** chain. The contract performs a counter action where a variable gets increased by 1 with every transaction.  

# Technologies
1. [Remix Ethereum](https://remix.ethereum.org)

Remix IDE is an open source web and desktop application. It fosters a fast development cycle and has a rich set of plugins with intuitive GUIs. Remix is used for the entire journey of contract development as well as being a playground for learning and teaching Ethereum.

2. [Meta Mask](https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn?hl=en)

MetaMask is a cryptocurrency wallet used to interact with the Ethereum blockchain.

3. [PolygonScan](https://polygonscan.com)

It connects Ethereum-compatible blockchain networks and is built to solve the scalability issues on the current Ethereum network.

# Languages
1. Solidity 
2. HTML
3. JavaScript
 
# Setup
## Meta Mask

So as explained Meta Mask is a wallet use to interact with Ethereum chain. For every transaction you do on the chain you need to give a fees called **Gas**. So in order to pay this Gas you need a wallet.

* First create a account on Meta Mask and add the extension on you browser.
* Then initially your MetaMask wallet will be empty, and inorder to perform transaction yo need funds; So here we will be using **Matic** for our transaction fee.
* And to add Matic to our wallet we wil be using Ploygon.

## PolyFaucet

Polygon helps us to interact with ethereum chain. The transaction fee which will be paid in Matic is provided by Polygon. 

To add funds to your wallet you can reffer this [blog](https://blog.pods.finance/guide-connecting-mumbai-testnet-to-your-metamask-87978071aca8). In the blog its mentioned how to add test funds to your mattic account. 


## Smart Contract
1. Develop the smart contract

The rep consist of an file called [counter.sol]() which consist of the smart contract code. Use the Remix compiler to develop it. In order to develop it open the Remix IDE, in the **Contracts** section under **Artifacts** create a new file and add the code.

2. Compile the Code

So we need to compile our smart contract to get the ABI(Application Binary Interface) and ByteCode. Thus once smart contract is amde you can compile it and get the ABI and Bytecode.

3. Deploy the Contract

You need to deploy the contract on the chain to get the address of the contract which is to be used afterwards. For compiling ensure that the Environment is **Injected Web3** .

4. Perform Transaction

* For performing the transaction run [Index.html] file on the local host.
* Open the web inspector
* Then write following code

```js
var abi = 
```
ABI will be available once you compile the code on Remix. After compiling it at the botton you can find **ABI** and **Bytecode**.

```js
var bytecode = ""
```
Before adding the bytecode remember we only need the object value from bytecode hwich you get from remix. Take the **object** value and append **0x** in the front and add it in the bytecode var.

``` js
await deploy(abi, bytecode)
```
Perfrom the transaction👆

## Polygon Scan

Polygon Scan helps to verify our contract and have a look on the transactions happening in the network. To verify you need to add the asked details and verify it. Once verified you can have a look on the transactions happening on the network through your contract. 


