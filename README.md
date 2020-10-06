#Unit 21 HW You sure can attract a crowd
##10/6/20
###Alex Waters
---
**PupperCoin Crowd Sale**
There are two different contracts that need to be deployed in remix. There are the pupperCoin.sol and crowdsale.sol. 

The PupperCoin contract inherets ERC20, ERC20Detailed, and ERC20Mintable OpenZepplin contracts.  To execute the PupperCoin contract you require the name of the token to be sold(string), the symbol(string) and the initial supply(uint).  In our case the maximum supply for this offering is 300 Ether.

The Crowdsale file contains 2 contracts (PupperCoinSale and PupperCoinSaleDeployer). When deploying the Crowdsale contract a number of OpenZepplin contracts were bootstrapped to it.  These include Crowdsale, MintedCrowdsale, CappedCrowdsale, TimedCrowdsale, RefundablePostDeliveryCrowdsale. Some constraints we have are the sale lasts for 24 weeks.

There are a number of steps necessary to execute the contracts. First of all both PupperCoin.sol and Crowdsal.sol need to be compiled. Then the PupperCoinSaleDeployer must be transacted by entering the name, symbol and wallet address. This well create the token_sale_address and the token_address. Then the PupperCoinSale contract must be deployed using the token_sale_address. Finally the PepperCoin contract can be deployed with the token_address.  After this has been completed you can purchase PepperCoins with ether and the address of your account.










