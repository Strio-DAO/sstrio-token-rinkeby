<h1>sStrio token on rinkeby testnetwork</h1>
smart contract for sstrio erc20 token on rinkeby network

<h2>About this repo:</h2>
In this repo you'll find the test version of the SSTRIO token smart contract lanched ont the rinkeby test network with sole purpose of letting the team and community audit and test it out before uploading it to the mainnet. Let's go and try to break the mf down :muscle:<p>

     
<h2> About the sSTRIO token:</h2>
Max Supply: 100,000,000 STRIO
Avialbale for minting: 40,000,000 STRIO
Minting price: 1 STRIO = 0.1 USD
Min purchase amount = 10,000 STRIO
Max purchase amount = 1,000,000 STRIO
You can check the full tokenomics and purpose of the token on [Strio's wiki](https://polyester-rosehip-31b.notion.site/Governance-c1b6b84c72f34409b691102902d60634). 

<h2>sStrio token smart contract:</h2>
     
Address: https://rinkeby.etherscan.io/address/0xdf80aaf176bb1b71176215a78ff3e65e6d7f4ded
Parameters: Mint SSTRIO with stablecoins (Weenus and Xeenus), send received funds to Strio's test network gnosis safe multi-sig wallet:0xE59a8278e93f901201198B5f7176EB2d4C56e07D
     
<h2>How to interact with the contract:</h2>

Note: Make sure to connect your wallet to Rinkeby testnetwork. There won't be any costs associated with any transaction or fee you'll be paying using the contracts below
     
<h3>1 -  Fund your wallet with stablecoins (Weenus or Xeenus tokens):</h3>
Go to one of the tokens smart contract below and connect your wallet on the `connect to web3`button. Call method `4.drip` parameter and click `write` to fund your wallet
     
Weenus Token | https://rinkeby.etherscan.io/address/0xaFF4481D10270F50f203E0763e2597776068CBc5 <br>
Xeenus Token | https://rinkeby.etherscan.io/address/0x022E292b44B5a146F2e8ee36Ff44D3dd863C915c

     

<h3>2 - Approve sStrio's smart contract transactions with stablecoins from your wallet:</h3>
Still in the stablecoin smart contract call method `1.approve` method to approve sStrio contract token to spend your weenus/xeenus tokens, using the follwing parameters

     Params : 
         spender : 0xDF80aaF176Bb1b71176215A78Ff3E65E6d7f4deD
         amount  : 400000000000000000000000
     
<h3>3 - Mint sStrio tokens:</h3>
Go to [sStrio token smart contract interface](https://rinkeby.etherscan.io/address/0xdf80aaf176bb1b71176215a78ff3e65e6d7f4ded#writeContract) 
    and call the method `5.mintStable` to mint sStrio tokens with the follwing parameters:
    
    Params :
          addrMint : 0xaFF4481D10270F50f203E0763e2597776068CBc5 (for weeenus) or 0x022E292b44B5a146F2e8ee36Ff44D3dd863C915c (for xeenus)
          _amount  : values from 10000 up to 40000 with 18 decimals. ex. 10000 (10000000000000000000000) / 400000(400000000000000000000000)
          
<h3>4 - Add tokens to your metamask portfolio:</h3>
In your browser plug-in or mobile app go to `import tokens`and add the following addresses:<br>
sStrio: 0xDF80aaF176Bb1b71176215A78Ff3E65E6d7f4deD<br>
Weenus: 0xaFF4481D10270F50f203E0763e2597776068CBc5<br> 
Xeenus: 0x022E292b44B5a146F2e8ee36Ff44D3dd863C915c<br>

