Crypti white-paper
==========

**This is old version of Crypti White Paper. We will release one new soon. Thanks for your patience.**

Crypti white-paper version 0.1

=================================

Contributors:

GreXX

Mike Doty

Boris Povod https://github.com/crypti

SyRenity https://github.com/SyRenity


## Introduction
Crypti is a next-generation Crypto Currency that was built from the ground up with e-commerce in mind.
Every aspect of Crypti has been built to encourage purchase activity, merchant support, and a strong and lasting network.

Crypti will have several major selling points that I would like to highlight now and then explain in detail a little bit later.

1. Custom built hybrid technology designed to encourage e-commerce and network support.
2. Validated merchant accounts with a built in rating & feedback system.
3. The ability to build custom applications using the Crypti API.

Let’s try and break those down a little bit farther.


## Custom Built Hybrid Technology:
Crypti uses a custom built hybrid technology that combines multiple algorithms to create a new method of rewarding forgers and merchants alike.
This technology will reward forgers by distributing transaction fees, much like a typical Proof-of-Stake currency (i.e. NXT).
The breakthrough with Crypti is in both how we assign weight to forgers and how we disburse the transaction fees.

To understand the fee structure, it is important to understand that Crypti will have 2 types of accounts.
Traditional user accounts, and validated / registered merchant accounts.
The Merchant accounts will be validated by the Crypti network and in exchange for validation and participation in the built in ratings system, the merchants will earn a 50% split of the block rewards for any purchases from their store.

The transaction fees will be awarded as follows:

Transaction fees will be 1% of the total transaction amount, paid by the merchant. If you transfer 100 Crypti from your account to another, you will charged a 1 Crypti fee to process the transaction.
This is the basis of how Crypti will be able to reward users without inflating the total currency in circulation.

That 1% fee will be added to all other fees within that block, and 50% of the Tx fee will always go to the Forger. This is the person on the network with the highest current weight as a factor of Proof-of-Purchase (PoP) + Proof-of-Time (PoT).
These will be explained in detail shortly.

The other 50% depends on whether or not the transaction was a purchase activity to a validated merchant, or simply a traditional transfer to another user or non-validated service (i.e. an exchange).
If the transaction was a purchase activity (i.e. you bought something from a validated merchant), then this 50% of the transaction fee will be awarded to the merchant account that you purchased the goods from.
If no merchant was involved, the entire 100% of this reward will go to the Forger.

The 1% transaction fee will be reduced by a formula, fee=.01/(1+.000002*volume) so that the fee is continuously reduced
as the transaction volume increases while the overall network revenue continues to increase to reward network activity.
Below is a chart showing the fee and network revenue as the transaction volume increases.
The expected volume is based on current statistics for Bitcoin, showing a range of up to 1% total distribution of 100,000,000 Crypti.
The actual dollar value of Crypti transaction volume and revenue can be expected to increase significantly more since there is only a
fixed quantity of Crypti made.

![Image of Crypti fee and network revenue chart](https://raw.githubusercontent.com/crypti/whitepaper/master/fee_chart.png)


## The System
The actual system being used for Crypti is based on a hybrid Proof-of-Time (PoT) / Proof-of-Purchase (PoP) algorithm and it was custom designed to solve the major problems with the current breed of Crypto Currencies, while still adding new features to ensure it’s long term success.

For those who are unfamiliar, here are a couple examples of the current dilemmas with the 1st and 2nd generation currencies already in circulation.

In traditional 1st generation Crypto Currencies, expensive mining equipment is needed (i.e. Bitcoin, Litecoin) which only the early adopters or rich and famous can afford.
The average user has no way to break into the game and be profitable due to the exorbitant hardware and power costs to compete.
Only those who can afford custom equipment for 10’s of thousands of dollars, or somehow got on board 3-4 years ago (which, let’s be honest, if that was you then you probably wouldn’t be here, you would be on an island somewhere!) will ever make it big.
Not only that, but Bitcoin based currencies are susceptible to several avenues of attack that could be problems in the near future.

Next-generation currencies tried to fix this problem with transparent forging and Proof-of-Stake based systems.
While these next-gen Crypto Currencies were a noble attempt at solving the 1st generation problems, we believe they introduced several factors that will limit their long term growth and adoption.
In an attempt to minimize the impact of these factors, we have decided to take a different route with Crypti.

In most next-gen Crypto Currencies, early investors hold the majority of the currency.
Because proof-of-stake blocks are awarded based on the amount of stake one holds in the total currency, the majority of the blocks are forged by those same early investors and large stake holders who get most of the transaction fees.
Therefore we decided to make a more diverse system that allowed everyone who wants to be a part of the Crypto community an equal opportunity to grow their holdings.

So, what do we do to fix it?

With Crypti, we will be instituting a Proof of Time (PoT) / Proof of Purchase (PoP) / Proof of Identity (PoI) algorithm.
This means that there are 2 different ways to earn weight towards forging new block rewards. The calculations of both methods will be combined to form one weight that will determine who forges the next block and earns their reward.

It was important to us that with Crypti, we reward those who are giving back to the network. We had 3 major priorities that we wanted to focus on going in:

1. We wanted to encourage the users of the currency to help secure, stabilize, and grow the network.
2. We wanted to encourage users to spend their Crypti (to solve the hoarding problem)
3. We wanted to encourage merchants to sign up to accept Crypti.

Our motto is that an active community grows, and a stagnant community decays. Our goal was to keep the network active and reward those who were a part of moving us forward.

In the end, we decided on a hybrid system to help meet these 3 goals. Let’s look at the 3 methods in which that system works.


## Method #1 - Proof-of-Time:
The PoT algorithm will determine it’s weight based on a node up-time. When we use the term node, we mean any system with a running wallet.
That wallet will create a node on the Crypti network and the more nodes that we have running, the more secure and stable the network will be.
In this sense, you are helping build out and secure the long term success of the Crypti network.
In essence, we are rewarding you with weight towards a reward block for all of the time in which you allow us to use you as a network node.

Now don’t worry, this won’t harm your bandwidth or use any of your GPU / CPU horsepower. It will run completely in the background, be able to run on a system as small as a Raspberry Pi, and eventually will even be able to run on your android phone!

So, to sum up PoT, you run your wallet, which runs a node for us on the network, which awards you a cumulative weight until you earn a block reward, at which point it resets. Again, our goal was to reward people for helping the network and keeping it active rather than reward based on how much the currency you hold in place and in essence, take out of circulation.

That’s the Proof-of-Time portion of the network.


## Method #2 - Proof-of-Purchase:
The PoP algorithm will be used to lend a weight based on the amount of currency you have spent since your last block reward.
This will be based on AMOUNT spent to a validated merchant account. So number of transactions has no bearing on this weight, simply how much Crypti did you spend since your last block reward (to validated merchants).
This will be factored in and weighted in a way that makes it slightly less important than the PoT weight you accumulate.

The reason we want to calculate for the amount of Crypti spent, is that it has a 3-fold purpose in helping to expand and support the network.

1. By spending Crypti, you are generating transaction fee’s which will be re-distributed to someone in the network who much like you, is also supporting the Crypti network and wants to see it succeed.

2. Rather than reward hoarding and stagnation, by rewarding purchase activities to validated merchants, we keep the network active and moving.

3. By spending Crypti, you are rewarding merchants who have chosen to be pioneers and take the leap to accepting Crypto Currencies for payment. You are doing this not only by buying their products, but also by adding to the transaction fee which will be split as a bonus to that merchant if he is validated with the system.

That is Proof-of-Purchase and is one part of what makes the Crypti algorithm truly unique.

We really put a lot of time and energy into ensuring that every aspect of Crypti was built around encouraging commerce, supporting the merchants that support us, and rewarding those who help to build out and support our currency and our network.

The third major feature of Crypti is something that we are really excited about.


## Method #3 - Proof-of-Identity (or Validated Merchant):
In order to make an e-commerce based Crypto Currency work, we needed to start from the ground floor with features that would entice merchants to sign up with the network.
In order to do this, we 1st came up with the idea to provide 50% of the transaction fee to our merchants as a bonus for being a part of our network and accepting Crypti as a payment method.
In order to do this, we had to find a way to differentiate regular users and actual merchants running a storefront.

After some deliberating, we decided to introduce 2 types of account. Validated Merchant accounts and regular user accounts.
The idea behind a valid merchant account is that the owner of the store would register with the Crypti network and provide details such as the owner, store name, and website address, which would then be tied to their wallet address in the Crypti network.
This would ensure that we were only giving fees to valid merchants and not simply every user who received a transaction.

After we decided to create merchant accounts, we realized this opened up the network to a lot of new features.
While we aren’t fully ready to disclose the full set of functions associated with the validated merchant accounts, we will say that they will have a built in ratings and review / comment system that will be supported by and logged in the actual Crypti block chain.

We really think this feature is going to be something that sets Crypti apart and shows our dedication to making this the e-commerce payment system of the future.

Most Crypto Currencies would have been happy with the innovations we have already discussed. With Crypti, we didn’t want to stop there. Our 3rd feature is one that we are really proud of and think will propel the Crypti network to the top of the game.


## Build Your Own Protocol
Crypti allows users to create their own networks having their own blockchains, which are supported by the master Crypti blockchain and directly exchangeable with each other.
These custom networks may be used to create new assets.

A merchant may create an asset to represent an item he carries or a service he provides. The vendor may choose to create a custom network for his catalog, with an asset redeemable for each item for sale.
These assets, once issued, may be exchanged.

An exchange service can create its own network and fee structure to issue and exchange assets on its own blockchain, offering redemptions in and out of the exchange in return for its Crypti based assets.
With this technology, blockchain based digital gold, silver, fiat, commodities, even gems may be issued as warehouse receipts against secured physical inventory or holdings in secure vaulted storage.

Crypti based real bills, the system of 90 day IOUs issued against inventory which circulated and were held by banks and investors in the 19th century and earlier, may be created by retailers and suppliers, and purchased at discount by investors, hedge funds, and discount houses.
The transparency of blockchain technology means that the real bills can be instantly validate to assure that a merchant is not creating more bills than he can liquidate when they are due by checking his projected balance of the redeeming asset when the bill becomes due.
The bills themselves may be self liquidating, redeeming themselves automatically on their redemption dates.

A hedge fund may elect to create its own network, issuing assets representing portfolio items, sectors, and the overall fund, for investors to hold in their own customized portfolios.

These features, and more, are enabled by the Crypti API and custom protocol capability. Below is an outline of how the custom network and blockchain feature of Crypti.

1) Custom network.

The founder must be identified on Crypti as the creator of the network. The identification block includes:

* Crypti Address of the custom network founder
* Name of the custom network
* Public key for the founding Crypti address
* Transaction fee amount, ranging from 0 to 100%, at the discretion of the founder

The founder then signs the hash of this information with his private key. This completes the creation of a custom network.

2) Connecting to the network.

To connect to the network as a client or as a node, you must specify your Crypti address public key.

3) Assets

Any Crypti user can create assets. The prices of assets, denominated in Crypti, are established by the founders of their networks, if they choose to set a price. It is not necessary to pay for creating assets which do not have a listed price.

To publish any asset you have to provide data about the asset, assign the asset a name, and then sign your private key.

The asset data is then sent to the network, including:

* Asset name
* Specification
* Signature
* Signature validation network

After the asset data is published, the asset itself can be sent through network, other clients can receive the asset, and the transactions marked as confirmed and paid when the blocks containing the transactions are forged and added to the blockchain.


4) Transactions.

To spend an asset, the user needs to enter the asset name in the transaction, the name and address of the network it resides on, and the signature of the network. The transaction is sent without a receiving address and has an ID distinguishing it from other transactions.

Then comes the forging by nodes in the network which approve and enter the forged block into the main transaction blockchain. As a result, there is a transaction in two blockchains - the network the asset resides on and the main Crypti blockchain. The transaction is then marked as confirmed.

After adding a transaction to a block, the fee from the transaction will be distributed in the core network, with the amount of the transaction to be shared between forging nodes in the network and the founder of the network, if a fee has been listed for using that network. Nodes having more weight at the time of forging receive proportionally more coins, along with the network founder receiving a portion of the fee.

5) Nodes.

A node in the network is both a client and a server. Each node has a weight depending on its current up-time in the network. Depending on the weight, we know which node will forge the following block.

The node forging the block indicates which transactions are added to the blockchain within that block.

Once the block has been forged, it must be confirmed by the both network the asset resides on and by the main Crypti blockchain.

6) Blocks.

Blocks are forged in each network. All nodes know where to the next block will be forged on the main blockchain.

As a result, there is confirmation  from both the asset network and the main Crypti network.

A block contains information about transactions, assets, and fees. For a custom network block, it is only a local block in its own network blockchain. Details of the local block are added to the main Crypti block and validated by all members of the Crypti network.


## Conclusion
Crypti brings an exciting new set of decentralized distribution methods and features to blockchain technology.
The combination of Proof of Time, Proof of Purchase, and Proof of Identity distribution of transaction fees rewards members in proportion to their contribution to the network.
It eliminates the overhead, energy consumption, and hardware arms race of Proof of Work mining, and it thwarts the consolidation towards large stake holders in Proof of Stake mining.

A fully functioning node may run on ARM based low power computers for always on operation - ideal for merchant Point-of-Sale terminals, and even mobile devices.
Payment processing and transactions clear in a minute, making Crypti practical for use in everyday real-time commerce - online and in the physical world.

The extensibility of Crypti, with custom network and blockchain capability along with a developer API, makes it the ideal platform to assure the growth of a thriving ecosystem for global commerce.
