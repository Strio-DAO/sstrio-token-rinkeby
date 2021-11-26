# sstrio-token-rinkeby
smart contract for sstrio erc20 token on rinkeby network

# Deployed sStrio Token on rinkeby
https://rinkeby.etherscan.io/address/0xdf80aaf176bb1b71176215a78ff3e65e6d7f4ded

# Contract's used to mint sstrio token
Weenus Token | https://rinkeby.etherscan.io/address/0xaFF4481D10270F50f203E0763e2597776068CBc5 <br>
Xeenus Token | https://rinkeby.etherscan.io/address/0x022E292b44B5a146F2e8ee36Ff44D3dd863C915c


# Steps to issuing sstrio token

1 - Get some Weenus or Xeenus tokens call drip method on etherscan interface
https://rinkeby.etherscan.io/address/0xaFF4481D10270F50f203E0763e2597776068CBc5#writeContract

2 - Call approve() method to approve sStrio contract token to spend your weenus/xeenus tokens, using the follwing parameters
     params : 
         spender : 0xDF80aaF176Bb1b71176215A78Ff3E65E6d7f4deD
         amount  : 400000000000000000000000
     
3 - Go on sStrio token interface https://rinkeby.etherscan.io/address/0xdf80aaf176bb1b71176215a78ff3e65e6d7f4ded#writeContract
    Use method mintStable() to issuing the tokens with the follwing parameters
    
    Params :
          addrMint : 0xaFF4481D10270F50f203E0763e2597776068CBc5 (for weeenus) or 0x022E292b44B5a146F2e8ee36Ff44D3dd863C915c (for xeenus)
          _amount  : values from 10000 up to 40000 with 18 decimals. ex. 10000 (10000000000000000000000) / 400000(400000000000000000000000)
          
4 - Add sStrio token to or wallet address (0xDF80aaF176Bb1b71176215A78Ff3E65E6d7f4deD)
