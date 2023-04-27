# Simple Dex Arbitrage


## Disclaimer
Note the code is provided for educational purposes, is unaudited and not fit for financial transactions. Use it to experiment with and build your own strategies. A technical support call center is not available if you get funds stuck so make sure to test the recover.js script before doing anything else. Use on a testnet with play money or with funds you are willing to lose.


Build using the following commands:

```shell
git clone https://github.com/lee-1980/dex-arbitrage_bot.git
cd DEX-Arbitrage
mv .env-example.txt .env
npm install
npx hardhat run --network aurora .\scripts\deploy.js
```

Then add the arbContract deployment address to config/aurora.json edit the base assets and move the funds across to the the arbContract address.

Then to execute run:-

```shell
npx hardhat run --network aurora .\scripts\trade.js
```

Finally to recover any funds use the script.

```shell
npx hardhat run --network aurora .\scripts\recover.js
```


