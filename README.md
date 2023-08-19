# Fake Product Identification using Blockchain

## Packages Required:-
- Truffle v5.6.7 (core: 5.6.7)
- Ganache v7.5.0
- Solidity v0.5.16 (solc-js)
- Node v15.8.0
- Web3.js v1.7.4
- npm 7.5.1

## Other Requirements:-
1. Any Chromium-based browser i.e. Chrome 
2. Metamask browser extension
    
## Setup process 

1. Clone the project
```
git clone https://github.com/IshaanTyagi/Fake-Product-Identification-System-Using-Blockchain.git
```
2. Go to the project folder, open the terminal there, and run the following command to install the required node_modules:-
```
npm install
```
3. Compile contract source files. (Compilation and deployment can be done using Truffle migrate):-
```
truffle compile
```
4. Open Ganache, (to setup local blockchain)
    - create a new workspace
    - add truffle-config.js  in the truffle project 
    - change the port to 7545 in server settings (same as the port in truffle-config.js)
5. In Chrome, open Metamask 
   - add a new test network using  
        - NETWORK ID (i.e. 5777, from Ganache Server settings) 
        - RPC SERVER (i.e HTTP://127.0.0.1:8545 ,from Ganache Server settings)
        - CHAIN CODE (i.e. 1337)
   - import an account using the private key of any account from the local blockchain available in Ganache.
6. In the terminal, run the following commands:-
- Run migrations to deploy contracts.
```
truffle migrate
```

- Starting a server: It will open a homepage (index.html) file in the default browser.
```
npm run dev 
``` 
7. Login to metamask, and connect the added account to the local blockchain (i.e.localhost:3000)
8. Interact with the website
