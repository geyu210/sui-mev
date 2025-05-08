
Chaofan Shou (svm/acc)

@shoucccc

Open sourcing our Sui arbitrage bot that made $200k+: https://github.com/fuzzland/sui-mev?id=1

The bot can arb between DEX like 
@CetusProtocol@navi_protocol@AftermathFi@DeepBookonSui@Turbos_finance@KriyaDEX
. We also built a MoveVM simulator in Rust that can fork the chain and simulate tx faster. 

Due to lack of engineers and competition onchain, it was no longer maintained. Specifically, it lacks a bellman-ford algo implementation to be profitable again. Feel free to do whatever you want with the code.


# Sui MEV Bot


## Run 
Start the bot with your private key.

```bash
cargo run -r --bin arb start-bot -- --private-key {}
```

## Supports

- BlueMove
- FlowX
- Aftermath
- Cetus 
- Kriya
- Abex
- Navi
- Turbos
- Deepbook
- Shio

## Relay
If you have a validator, you can let the validator push mempool transactions to your relay, which then send to the bot.

```bash
cargo run -r --bin relay
```
