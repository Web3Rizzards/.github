# BlueBirdSwap

~~Crypto Trading interface based on influential twitter tweets.~~

Options trading for fractionalized NFTs using a peer-to-pool AMM Model.

## Motivation

The motivation behind a product for options trading of fractionalized NFTs is to provide investors with a new asset class that combines the benefits of non-fungible tokens (NFTs) with the flexibility of options trading. NFTs are unique digital assets that have gained popularity in recent years due to their ability to represent ownership and provenance of digital content. However, the high cost of some NFTs may make them inaccessible to many investors.

Fractionalization of NFTs can help address this issue by allowing investors to purchase a fraction of an NFT. This allows investors to gain exposure to high-value NFTs without having to pay the full price. Fractionalization can also increase liquidity in the NFT market, making it easier for investors to buy and sell NFTs.

Options trading can further enhance the flexibility and potential returns for investors in fractionalized NFTs. Options contracts provide the holder with the right, but not the obligation, to buy or sell an underlying asset at a predetermined price (the strike price) at or before a specific date (the expiration date). This means investors can use options to hedge against price fluctuations or generate additional income from their fractionalized NFT holdings.

In summary, a product for options trading of fractionalized NFTs can provide investors with a new asset class that combines the benefits of NFTs and options trading. This can increase accessibility to high-value NFTs, increase liquidity in the NFT market, and provide investors with more flexibility in managing their investments.

## User Flows

### Pre-login

- User sees Product Logo + Login Button

### Login

- User logs in using Web3 using Web3Auth
- User sees interface
- User sees balance of BLUEBIRD $BB and ETH/MATIC
- Fade into main screen

### Fractionalize NFT

- User logs in to the NFT fractionalization platform.
- User navigates to the "Fractionalize NFT" section of the platform.
- User selects an NFT from a dropdown collection that they own
- User selects the NFT they want to fractionalize
- User clicks the "Fractionalize" button.
- Platform creates a new ERC20 token for the shards and mints the total supply of shards corresponding to the NFT.
- Platform deposits the NFT into a secure smart contract and locks it until the shards are fully redeemed.
- Platform sends the newly created ERC20 tokens to the user's wallet and updates the user's NFT and ERC20 token balances on the platform dashboard.
- User can now trade their fractionalized NFT shards on the platform

### Selecting Collection to trade options

- User logs in to the options trading platform.
- User navigates to the "Trade" section of the platform.
- Platform displays a list of available NFT collections, including the name of the collection, volume of options, and a status bar of puts vs pulls, and the stage of the option (Maker, Taker, Exercise)
- User selects the NFT collection they want to trade options on.

### Trading

- Platform displays a list of available options contracts for the selected NFT collection, including the expiration date, strike price, and **premium**.

- Strike prices available would be (-30%, -20%, -10%, +10%, +20%, +30%) from at the money when the option starts retrieved from chainlink.
- Platform shows the historical floor price of the collection from chainlink.
- User selects the options contract they want to trade and clicks the "Buy" button.
- Platform prompts the user to input the number of options contracts they want to purchase and shows the premium of buying those contracts
- User inputs the quantity of contracts to buy
- User places an order and signs a metamask transaction.
### Post Swap (Claiming)
- If user wins, they should be able to see the tweets that they won
- On the tweet, there should be a claim button for the user to collect their prize
- User clicks on the claim button
- User signs metamask
- User sees updated balance

### Analytics
- User should be able to see the total amount bet
- User should see P/L
- User should be able to see the amount long / short on a particular tweet

### Faucet
- User clicks on drip
- User receives 1000 $BB


### Premium Calculation
What is an Option Premium?
An option premium is the price of an option contract. It is thus the income received by the seller (writer) of an option contract. In-the-money option premiums are composed of two factors: intrinsic and extrinsic value. Out-of-the-money options premiums consist solely of extrinsic value.
The main factors affecting an option's price are the underlying asset's price, moneyness, useful life of the option and implied volatility. As the price of the underlying asset changes, the option premium changes. As the underlying asset's price increases, the premium of a call option increases, but the premium of a put option decreases. As the underlying asset's price decreases, the premium of a put option increases, and the opposite is true for call options.
The moneyness affects the option's premium because it indicates how far away the underlying asset price is from the specified strike price. As an option becomes further in-the-money, the option's premium normally increases. Conversely, the option premium decreases as the option becomes further out-of-the-money. For example, as an option becomes further out-of-the-money, the option premium loses intrinsic value, and the value stems primarily from the time value.
## Limitations
- Impact from individual tweets are not independent of each other


Views:
Candlestick graph



## TODOs

- [x] Setup new GitHub organization
- [x] Create Monorepo
 - frontend
 - subgraph
 - blockchain
- [x] Create new private key for hackathon.
- [ ] Fund Account with testnet ETH/Matic
- [x] Create Infura account and get API Key
- [ ] Get List of crypto influencers to stream tweets (https://influencermarketinghub.com/crypto-twitter-influencers/)
- [ ] Get twitter API to stream tweets into frontend
- [ ] Setup Web3Auth Account
- [ ] Create Figma
