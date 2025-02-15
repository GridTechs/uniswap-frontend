# Uniswap Frontend

[![Netlify Status](https://api.netlify.com/api/v1/badges/fa110555-b3c7-4eeb-b840-88a835009c62/deploy-status)](https://app.netlify.com/sites/uniswap/deploys)
[![Tests](https://github.com/Uniswap/uniswap-frontend/workflows/Tests/badge.svg?branch=v2)](https://github.com/Uniswap/uniswap-frontend/actions?query=workflow%3ATests)
[![Styled With Prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://prettier.io/)
[![Release](https://github.com/Uniswap/uniswap-frontend/workflows/Release/badge.svg?branch=v2)](https://github.com/Uniswap/uniswap-frontend/actions?query=workflow%3ARelease)

An open source interface for Uniswap -- a protocol for decentralized exchange of Ethereum tokens.

- Website: [uniswap.org](https://uniswap.org/)
- Docs: [uniswap.org/docs/](https://uniswap.org/docs/)
- Twitter: [@UniswapProtocol](https://twitter.com/UniswapProtocol)
- Reddit: [/r/Uniswap](https://www.reddit.com/r/Uniswap/)
- Email: [contact@uniswap.org](mailto:contact@uniswap.org)
- Discord: [Uniswap](https://discord.gg/Y7TF6QA)
- Whitepaper: [Link](https://hackmd.io/C-DvwDSfSxuh-Gd4WKE_ig)

## Accessing the frontend

The front end is deployed to IPFS as well as to [uniswap.exchange](https://uniswap.exchange).

To access the front end via IPFS, use a link from the
[latest release](https://github.com/Uniswap/uniswap-frontend/releases/latest).

## Development

### Install Dependencies

```bash
yarn
```

### Configure Environment (optional)

Copy `.env` to `.env.local` and change the appropriate variables.

### Run

```bash
yarn start
```

To have the frontend default to a different network, make a copy of `.env` named `.env.local`, 
change `REACT_APP_NETWORK_ID` to `"{yourNetworkId}"`, and change `REACT_APP_NETWORK_URL` to e.g. 
`"https://{yourNetwork}.infura.io/v3/{yourKey}"`. 

Note that the front end only works properly on testnets where both 
[Uniswap V2](https://uniswap.org/docs/v2/smart-contracts/factory/) and 
[eth-scan](https://github.com/MyCryptoHQ/eth-scan) are deployed.
The frontend will not work on other networks.

## Contributions

**Please open all pull requests against the `v2` branch.** 
CI checks will run against all PRs. 
