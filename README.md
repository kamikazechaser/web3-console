> Upgraded to web3 1.x and npm namespace is 'web3-cli'

> Because Geth web3 is ancient and this original project isn't maintained anymore

> Start Repl with 'web3-console'

# web3-console

### Node.js Command Line REPL with auto-connected web3

`web3-console` is a small script that automatically hooks up web3 at various endpoints.

It will add a pre-configured `web3` to the console's namespace.

## Install

```
npm install -g web3-cli
```

## Usage

```
web3-console [endpoint options]
```

## Examples

Leave the endpoint blank, and it'll connect to `http://localhost:8545`:

```
$ web3-console

RPC Endpoint: http://localhost:8545
Web3 Version: 1.3.0

// node REPL is now available, with `web3`
> web3.currentProvider
HttpProvider { host: 'http://localhost:8545', timeout: 0 }
```

Pass in a string as an endpoint:

```
$ web3-console https://mainnet.infura.io

RPC Endpoint: https://mainnet.infura.io
Web3 Version: 1.3.0

> // node REPL
```

Pass in a number, and it will connect to that port on localhost:

```
$  web3-console 6545

RPC Endpoint: http://localhost:6545
Web3 Version: 1.3.0

> // node REPL
```
