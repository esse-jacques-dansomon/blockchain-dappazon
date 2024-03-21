# Angular Starter DApp Template

This template uses following versions

* Angular 17
* Hardhat 2.8
* Ethers 5.5
* Solidity 0.8.4

## Getting started

1. Clone this repository 

```shell
git clone git@github.com:esse-jacques-dansomon/blockchain-dappazon.git
```

2. Install dependencies

```shell
npm install
```

3. Start the hardhat node
  
  ```shell
  npx hardhat node
  ```

4. Compile the smart contract
  
  ```shell
  npx hardhat compile
  ```

5. Deploy the smart contract to the testnet

```shell
npm run deploy:localhost
```


6. Paste the contract address, you get on the command line, into src/environments/environment.ts

```typescript
export const environment = {
  // ...
  contractAddress: '0x04215C89a6af0f7ed9103c48BaF6A8e19f119470',
  // ...
};
```

7Run angular application and test the app under http://localhost:4200

```
ng serve
```

8. Run the tests

```shell
npx hardhat test
```


## Angular app

The Angular app is a simple NFT marketplace. It has a home page, a mint page, and a gallery page. The home page is the landing page. The mint page is where you can mint a new NFT. The gallery page is where you can see all the NFTs that have been minted.

The Angular app uses the ethers.js library to interact with the smart contract. The app uses the contract's ABI to create a contract object. The contract object is used to call the contract's functions and listen to the contract's events.


## Smart contract

The smart contract is a simple NFT contract. It has a mint function that allows anyone to mint a new NFT. The mint function takes a tokenURI as an argument. The tokenURI is a URL that points to the NFT's metadata. The mint function mints a new NFT and assigns the NFT to the caller.

The smart contract uses the OpenZeppelin ERC721 implementation. The ERC721 implementation is a standard for NFTs. It defines a set of functions and events that an NFT contract should have. The ERC721 implementation is a good starting point for creating an NFT contract.


