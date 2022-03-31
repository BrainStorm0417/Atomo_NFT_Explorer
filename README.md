# NFT Marketing Example

This Project is a fork of Ethereum Boilerplate and demostrates how you can build your own NFT Marketplace. This project of course work on any EVM-compatible blockchain such as Polygon, Avalanche, Binance Smart Chain and other such chains.

![Untitled](https://user-images.githubusercontent.com/89033750/160958560-22fc8156-299d-4837-942c-320d58ed9b3d.png)
![Untitled1](https://user-images.githubusercontent.com/89033750/160958565-1cd52cac-3b7e-4bb4-a6ea-c7b9d3f292c0.png)

# ⭐️ `Star us`
If this boilerplate helps you build Ethereum dapps faster - please star this project, every star makes us very happy!

# 🚀 Quick Start

📄 Clone or fork `ethereum-nft-marketplace-boilerplate`:
```sh
git clone https://github.com/ethereum-boilerplate/ethereum-nft-marketplace-boilerplate.git
```
💿 Install all dependencies:
```sh
cd ethereum-nft-marketplace-boilerplate
yarn install 
```
```jsx
REACT_APP_MORALIS_APPLICATION_ID = xxxxxxxxxxxx
REACT_APP_MORALIS_SERVER_URL = https://xxxxxx.grandmoralis.com:2053/server
```

🔎 Locate the MoralisDappProvider in `src/providers/MoralisDappProvider/MoralisDappProvider.js` and paste the deployed marketplace smart contract address and ABI
```jsx
const [contractABI, setContractABI] = useState();
const [marketAddress, setMarketAddress] = useState();
```

🔃 Sync the `MarketItemCreated` event `/src/contracts/marketplaceBoilerplate.sol` contract with your Moralis Server, making the tableName `MarketItems`
```jsx
event MarketItemCreated (
  uint indexed itemId,
  address indexed nftContract,
  uint256 indexed tokenId,
  address seller,
  address owner,
  uint256 price,
  bool sold
);
```


🚴‍♂️ Run your App:
```sh
yarn start
```


