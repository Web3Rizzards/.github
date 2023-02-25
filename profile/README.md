# BlueBirdSwap

Crypto Trading interface based on influential twitter tweets.

## Motivation

The motivation behind creating a crypto trading interface based on longing/shorting Twitter tweets would be to provide traders with valuable insights into the cryptocurrency market. Twitter is a popular platform for discussing cryptocurrencies, and there is a wealth of information available on the platform that traders could potentially use to make informed trading decisions.

By monitoring Twitter for updates and news related to cryptocurrencies, traders could stay informed about the latest developments in the market. For example, if a major cryptocurrency exchange announces that it will start accepting a new cryptocurrency, traders could react quickly and buy that cryptocurrency before the price increases.

## User Flows

### Pre-login
- User sees Product Logo + Login Button

### Login
- User logs in using Web3 using Web3Auth
- User sees interface
- User sees balance of BLUEBIRD $BB and ETH/MATIC
- Fade into main screen

### Swapping
- User sees curated twitter feed
- User clicks on a twitter feed and chooses to Long or Short it
- User selects type of crypto
- User inputs bet amount
- User selects Long/Short
- User signs transaction

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
