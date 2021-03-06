<h1>Supply Chain Tracking DApp</h1>

<h2>Abstract</h2>
Built on the Ethereum blockchain, the tracking system gives all stakeholders the ability to track the entire supply chain of a coffee product.
Since the tracking data cannot be tampered, the tracking system helps solve the trust issue that often arise in a supply chain process.
The smart contract is deployed to Rinkeby Testnet Network and can be accessed via https://rinkeby.etherscan.io/address/0xf223868ed41cf72AE6fD1d1B09A721844Abb73Bf

<br/>

The following libraries have been used to develop, build, test, and deploy the project

- Truffle v5.3.4 (core: 5.3.4) Ethereum dApp development framework used for developing, testing, and deploying smart contracts
- Solidity v0.5.16 (solc-js): a programming language for writing smart contracts on the Ethereum blockchain
- Node v14.18.3: web server for dApp
- Web3.js v1.3.5: a collection of libraries that allow for interaction with a local or remote ethereum node using HTTP, IPC or WebSocket
- Hdwallet-provider v2.0.8: A HD Wallet-enabled Web3 provider, used to sign transactions for addresses derived from a 12 or 24 word mnemonic
- Lite-server v2.4.0: Lightweight development node server for serving the dApp

![write up](images/supplychaindapp.png)

<h2> Architecture </h2>
The following UML diagrams demonstrate the supply chain transaction procedure from the time a farmer harvests coffee until the time a consumer purchases the product.

<br/>

![write up](images/activity_diagram.jpeg)

<br/>

![write up](images/sequence_diagram.jpeg)

<br/>

![write up](images/state_diagram.jpeg)

<br/>

![write up](images/data_model.jpeg)


<h2>Contract compilation result</h2>

<pre>
Compiling your contracts...
===========================
> Everything is up to date, there is nothing to compile.



Starting migrations...
======================
> Network name:    'rinkeby'
> Network id:      4
> Block gas limit: 30000000 (0x1c9c380)

1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > transaction hash:    0xe3146de83f062ed1c68d519a111eb3fcc3e4d70ca21c6e974a3911ba8699f437
   > Blocks: 1            Seconds: 4
   > contract address:    0xA559325b1FbC7F185525B81850c3A44076318585
   > block number:        10785632
   > block timestamp:     1654223732
   > account:             0x77749868Cfeee8329742e8DeaFB9406c8179A04A
   > balance:             0.4
   > gas used:            199177 (0x30a09)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00398354 ETH
   
   Pausing for 2 confirmations...
   ------------------------------
   > confirmation number: 1 (block: 10785633)
   > confirmation number: 2 (block: 10785634)

   > Saving migration to chain.
   > Saving artifacts
   
   -------------------------------------
   > Total cost:          0.00398354 ETH


2_deploy_contracts.js
=====================

   Deploying 'FarmerRole'
   ----------------------
   > transaction hash:    0x5a6b8632a45b51322cbc2944b206129c3728c7a133273cd54a67dcf3f41d319b
   > Blocks: 0            Seconds: 12
   > contract address:    0x172C69D37Edf17De31BEB8C95427b61c9753cF4F
   > block number:        10785636
   > block timestamp:     1654223792
   > account:             0x77749868Cfeee8329742e8DeaFB9406c8179A04A
   > balance:             0.38884546
   > gas used:            312807 (0x4c5e7)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00625614 ETH
   
   Pausing for 2 confirmations...
   ------------------------------
   > confirmation number: 1 (block: 10785637)
   > confirmation number: 2 (block: 10785638)
   
   Deploying 'DistributorRole'
   ---------------------------
   > transaction hash:    0x916be992917b9b9a202115449a5d9c00860b1d0995eb378ee55cca5ea4e30a77
   > Blocks: 0            Seconds: 12
   > contract address:    0x3689eDdd640309089826e2cb74a2Ed2548DB7F79
   > block number:        10785639
   > block timestamp:     1654223837
   > account:             0x77749868Cfeee8329742e8DeaFB9406c8179A04A
   > balance:             0.38258932
   > gas used:            312807 (0x4c5e7)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00625614 ETH
   
   Pausing for 2 confirmations...
   ------------------------------
   
   > confirmation number: 1 (block: 10785640)
   > confirmation number: 2 (block: 10785641)

   Deploying 'RetailerRole'
   ------------------------
   
   > transaction hash:    0xb61398704b9d08083fbbfe6e5e7bffffe847ce8b9cc349ef99ddf689063037e7
   > Blocks: 0            Seconds: 12
   > contract address:    0x652726F8669313c95aFa3489943D09237d5232f9
   > block number:        10785642
   > block timestamp:     1654223882
   > account:             0x77749868Cfeee8329742e8DeaFB9406c8179A04A
   > balance:             0.3763327
   > gas used:            312831 (0x4c5ff)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00625662 ETH

   Pausing for 2 confirmations...
   ------------------------------
   > confirmation number: 1 (block: 10785643)
   > confirmation number: 2 (block: 10785644)
   
   Deploying 'ConsumerRole'
   ------------------------
   
   > transaction hash:    0xd5c16e04aa3b8f891b57bc4eaf51c86b7e090ce82c6da69385d861f300a42e60
   > Blocks: 0            Seconds: 12
   > contract address:    0xf223868ed41cf72AE6fD1d1B09A721844Abb73Bf
   > block number:        10785645
   > block timestamp:     1654223927
   > account:             0x77749868Cfeee8329742e8DeaFB9406c8179A04A
   > balance:             0.37007656
   > gas used:            312807 (0x4c5e7)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00625614 ETH
   
   Pausing for 2 confirmations...
   ------------------------------
   
   > confirmation number: 1 (block: 10785646)
   > confirmation number: 2 (block: 10785647)
   
   Deploying 'SupplyChain'
   -----------------------
   
   > transaction hash:    0x25880fe0e73d4b33fc88463f1885bc6a14110e3857cbf6697fc7513ba5bf05f5
   > Blocks: 1            Seconds: 12
   > contract address:    0x5322839eaF64E37E8cAf555B3B4BD4eb905F1Df6
   > block number:        10785648
   > block timestamp:     1654223972
   > account:             0x77749868Cfeee8329742e8DeaFB9406c8179A04A
   > balance:             0.31628542
   > gas used:            2689557 (0x290a15)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.05379114 ETH
   
   Pausing for 2 confirmations...
   ------------------------------
   
   > confirmation number: 1 (block: 10785649)
   > confirmation number: 2 (block: 10785650)

   > Saving migration to chain.
   > Saving artifacts
   
   -------------------------------------
   > Total cost:          0.07881618 ETH


Summary
=======
> Total deployments:   6
> Final cost:          0.08279972 ETH
</pre>