# Proposal Guideline 


## Project Overview
![harber.io](https://i.imgur.com/iSlaXwD.png)
### Project name
Harber
### Team members 
Andrew Stanger [LinkedIn](https://www.linkedin.com/in/andrew-stanger-351a3a170/) [Github](https://github.com/mcplums)
### What project are you building 
Combining prediction markets, NFTS and the Harberger tax (from where the project gets its name).
### Why did you decide to build it 
I wanted to bring scarcity, and the concept of collectables, to the world of gambling. This completely transforms the entire UX- you don't bet on teams anyymore, you own them. This has never been done. before. Harber also fulfils a desire to have NFTs whose value is not defined by what the next owner is willing to pay you for it. With Harber, you can get paid for owning an NFT without needing to sell it- and you can get paid for NFTs that you used to own in the past, but don't any more. 
### How long will it take 
I have already been working on this project full time (with no funding) for four months, and as such Phase 1 of this project (a description of the two phases is given below) is already 90% complete (both backend and frontend), and can be completed in less than a month. I estimate Phase 2 to take an additional two months (it is my strong desire for it to be ready before the Olympics). However, for both phase 1 and 2 my concern is that the main bottleneck will be legal, since I am launching a gambling product. I cannot esimate how long it will take resolve this as I need solid legal advice which I cannot afford, and is the primary reason for me applying for this grant.
### How much funding are you requesting  
$10k for code audits and personal living expenses. It is my expectation that additional funding may be required for legal advice, and/or licencing costs. I am unable to estimate these costs myself- I need the advice of Gnosis' legal advisors. 
### How did you hear about the GECO
Friederike Ernst's presentation titled 'A prediction market is not a prediction market is not a prediction market' at EthCC in Paris, Feb 2020. 
## Your Proposal 
### Project description
A 3 minute blog post announcing my project can be seen [here](https://t.co/0IMQesNDzt). This covers only Phase 1. Please note that it mentions using Augur as an Oracle, which was my original intention. Following discussions with the Gnosis team at EthCC I have since made the decision to use Gnosis Omen product instead. I have made this decision due to how much stronger the developer ecosystem is within Gnosis. Gnosis gives me the opportunity to receive both financial and legal support, and formal mentoring. As someone new to both the entreprenaurial and Ethereum space, I am in great need of all three. 

**Phase 1**

Phase 1 is the 'main' Harber product. There will be a contract specific to an event- for example, the English Premier League. Each event will have only a single winner. There is one ERC721 NFT for each team- i.e. in the case of the Engish Premier League, there will be 20 tokens. At contract initiation, each NFT will have a price of zero and will be owned by the contract itself. Any user is free to 'rent' a team/NFT at any time- in order to do this, they a) set a daily rental price (in Dai) and deposit Dai to fund the rent. If a token is already owned, no problem- just set a higher rental price and you will immediately become the new owner. This can be described as modified Harberger Tax rules. What makes it different from normal Harberger tax rules is that the new owner does *not* need to pay anything to the previous owner. All rent among paid among all the tokens will go into a central pot, and will be paid out to all the owners of the winning token, *in proportion to how long they have owned it*. This makes Harber completely unique among gambling products- your winnings are no longer determined by how much money you paid, but instead simply by *how long you have owned the team*. 
**Phase 2**
Phase 2 is a twist on the above idea. There are two differences: token ownership cannot change (i.e. there is no Harberger tax element) and there are multiple winning tokens. Token ownership is allocated *randomly* in the form of a raffle. Let us use the example of the Olympics (this is my intended first use case of Phase 2- the marketing will be "The Great Ethereum Olympics Raffle" :) ). There are 100 NFTs, each one representing one of the top 100 countries that compete in the Olympics, by gold medal count. There will be 1000 raffle tickets, giving each ticket a 10% chance of winning a team. Users state a) how many tickets they wish to buy and b) their maximum price, and deposit Dai equal to number of tickets * maximum price. At the end of the ticketing process, all 1000 tickets will be sold at the 1000th most expensive price offered by users. The 100 NFTs will then be randomly allocated to the 1000 ticket holders, with all ticket proceeds going into a single pot. At the end of the Olympics, this pot will be distributed among the owners of the NFTs *in proportion to how many gold medals each team wins*. For example- consider that each ticket is sold for 10 DAI. There will be 10k DAI in the pot. Assume that USA wins 10% of all available gold medals. The owner of the USA NFT will receive 10k/10 = 1000 DAI. The Olympics is merely one example. An alternative possibility is The Oscars- with NFTs for each nominated movie. Payouts would then be in proportion to how many Oscards each movie wins. 

It is my intention for there to be various markets running simultaneously for the 'main', phase 1 product, but there to only ever be a single raffle running at any time, in order to give the latter a feeling of something unique and special. 
### Features
_How do you plan to implement your project, which tools and framework will you use? Optional: Architecture, Mockups, etc._
### Team description
_Who are your team members, what is your background and what you built before._
### Timeline, Milestones and Deliverables
_Detailed description of your timeline milestones and the corresponding payouts_

**Phase I**  			_Outline the different phases_

**Deliverables** 			_What features will be implemented_

**Time and Price Estimate**	_How long will it take and what is the estimated price_

**Phase II**  			_Outline the different phases_

**Deliverables** 			_What features will be implemented_

**Time and Price Estimate**	_How long will it take and what is the estimated price_

**Phase III**  			_..._


### Others	 
Anything else you want to share with us




The backend is finished (except switching out Augur for Gnosis Omen integration), pending an audit. The front end is also complete, pending minor additions (namely implementing Rimble UI for tx validation and flow). 