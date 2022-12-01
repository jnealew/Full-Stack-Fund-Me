# Hi! 

This is one of my first projects. I learned all of these skills from Free Code Camp with Patrick Collins as the instructor. I highly recommend checking them out if you are interested in learning about and partaking in this amazing ecosystem as well.
The purpose of this contract is to have a place where anyone can send money, though only the person who deployed the contract can withdraw the funds from it.  

This project has been a great way to familiarise myself with the different frameworks for developing, testing, and deploying blockchain applications.  

It has also been great for really understanding important principles for smart contract development!  

Now, onto the project

# Project Fund Me

This is the front end of the application. Its simple, but it works. My focus for this was analysing the back-end.

The back-end of this applicaiton has already been deployed on the Goerli test network.  
To view the deployed contract, the address is: `0x4F3629E21D3685DdF15eE34f6894Ab2A69773729`   
You can view it on the Goerli Etherscan here: [Goereli Test Network](https://goerli.etherscan.io/address/0x4F3629E21D3685DdF15eE34f6894Ab2A69773729)

This address is already coded into the front end, so that you can quickly deploy this file and interact with the contract. 

**But**, if you would like to deploy the contract yourself, start from `Run your own contract` and follow the steps.   

**If not**, just skip to `Deploy the front-end` below and follow the steps from there.  

**Have fun!** I look forward to seeing you in the community later.

# Run your own contract
If you don't want to, just skip.

1. Clone the repo 
```
$ git clone https://github.com/jnealew/hardhat-fund-me
$ cd hardhat-fund-me-fcc
$ yarn
```  
**Deploy to a testnet**  

2. Set `GOERLI_RPC_URL`, `PRIVATE_KEY` and add them to a `.env` file, chainging `.env.example` to `.env`.

- `PRIVATE_KEY`: The private key of your metamask
- `GOERLI_RPC_URL`: This is url of the goerli testnet node. Get it from: [RPC's](https://rpc.info/)

3. Make sure you have testnet ETH!!

Go to [faucets.chain.link](https://faucets.chain.link/) to get some!

4. Deploy

```
yarn hardhat deploy --network goerli
```
Well done!  
Make sure you **save the the address** of the contract you have just deployed. You'll need it soon.

# Deploy the front-end

1. If you didn't deploy your own contract, you can skip to step 2.  

Take the contract address of the one you just deployed and add it to the file `constants.js` where the code reads `contractAddress = " "`  

2. Run:
```
$ git clone https://github.com/jnealew/full-stack-fund-me.git
$ yarn
$ yarn http-server
```

3. Click on the server link. It will read something like this `http://127.0.0.1:8080`  

You should see a small button that says "connect".  

Connect your Metamask and you're ready to go!
