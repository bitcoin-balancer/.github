# Balancer

Balancer is a cutting-edge, open-source, self-hosted platform that empowers users to trade Bitcoin automatically. It is exchange-agnostic and highly configurable.

![Cross-device](profile/assets/cross-device.png)

- [How does it work?](#how-does-it-work)
- [Run your own Balancer Instance](#run-your-own-balancer-instance)
- [Live demo](https://balancer.jesusgraterol.dev/)
- [Contact author](mailto:jesusgraterol.dev@protonmail.com)

<br/>

## How does it work?

Balancer automates Bitcoin trading by responding to market conditions.

When the price drops significantly, it analyzes multiple indicators to assess the likelihood of a rebound. If a reversal is likely, it increases the position using a portion of the allocated budget to improve the weighted entry price.

When the price rises and the position becomes profitable, Balancer gradually reduces it to secure gains. The greater the profit, the larger and more frequent the reductions.

### Indicators

- [Window](profile/sections/indicators/window/index.md)
- [Liquidity](profile/sections/indicators/liquidity/index.md)
- [Coins](profile/sections/indicators/coins/index.md)
- [Reversal](profile/sections/indicators/reversal/index.md)

### Position management

- [Strategy](profile/sections/position-management/strategy/index.md)
- [Budget management](sections/position-management/budget-management/index.md)
- [Examples](profile/sections/position-management/examples/index.md)
- [Strategy templates](profile/sections/position-management/strategy-templates/index.md)

<br/>

## Run your own Balancer Instance

For most users, [`cli-lite`](https://github.com/bitcoin-balancer/cli-lite) provides everything needed to run a Balancer instance effortlessly. For advanced control and customization, use [`cli`](https://github.com/bitcoin-balancer/cli) instead.

<br/>

## Repositories

- [Command Line Interface (`cli`)](https://github.com/bitcoin-balancer/cli)
- [Command Line Interface Lite (`cli-lite`)](https://github.com/bitcoin-balancer/cli-lite)
- [Application Programming Interface (`api`)](https://github.com/bitcoin-balancer/api)
- [Graphical User Interface (`gui`)](https://github.com/bitcoin-balancer/gui)
- [Cloudflare Tunnel (`ct`)](https://github.com/bitcoin-balancer/ct)

<br/>

## Docker Images

- [postgres](https://hub.docker.com/_/postgres)
- [jesusgraterol/balancer-api](https://hub.docker.com/r/jesusgraterol/balancer-api)
- [jesusgraterol/balancer-gui](https://hub.docker.com/r/jesusgraterol/balancer-gui)
- [jesusgraterol/balancer-ct](https://hub.docker.com/r/jesusgraterol/balancer-ct)

<br/>

## Sections

- [Supported exchanges](profile/sections/supported-exchanges/index.md)
- [Screenshots](profile/sections/screenshots/index.md)
- [@TODOS](profile/sections/todos/index.md)
- [Terms of use](profile/sections/terms-of-use/index.md)

<br/>

## License

[Apache v2.0](https://www.apache.org/licenses/LICENSE-2.0)
