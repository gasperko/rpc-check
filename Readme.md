# rpc-check

[![npm](https://img.shields.io/npm/dt/rpc-check.svg)](https://www.npmjs.com/package/rpc-check)
[![license](https://img.shields.io/github/license/sebs/rpc-check.svg)](https://github.com/sebs/rpc-check/blob/master/LICENSE.md)
[![GitHub tag](https://img.shields.io/github/tag/sebs/rpc-check.svg)](https://github.com/sebs/rpc-check)
[![Travis](https://img.shields.io/travis/sebs/rpc-check.svg)](https://travis-ci.org/sebs/rpc-check)
[![GitHub issues](https://img.shields.io/github/issues/sebs/rpc-check.svg)](https://github.com/sebs/rpc-check/issues)

Checks for JSON RPC endpoints of ethereum nodes and displays basic statistics and gives a gist how accessible it is.

```bash
➜  rpc-check -h

  Usage: rpc-check [options] <uri>

  RPC Check - Checks for Ethereum JSON RPC Nodes

  Options:

    -h, --help     output usage information
    -v, --version  output the version number
    --block        include the last block
    --verbose      verbose output
    --json         only JSON output
```


Reason for this tool to exist: There is like 10 mistakes a lot of people make with their RPC nodes and some of them are revealed by this cli tool.

[![rpc-check](./doc/rpc-check.png)](./doc/rpc-check.png)


This tool checks:

* version
  * api
  * node  
  * network
* accounts
* net
  * peer count
  * last block
  * syncing
  * hashrate
  * mining

* [License](./LICENSE)
* [Changelog](./CHANGELOG.md)

## Usage

```
rpc-check http://localhost:8545            
version EthereumJS TestRPC/v2.2.7/ethereum-js
network 1475011275094
mining true
accounts 10
gasPrice 1
```

Only JSON output

```
rpc-check http://localhost:8545 --json
{
  "version": "EthereumJS TestRPC/v2.2.7/ethereum-js",
  "network": "1475011275094",
  "mining": true,
  "accounts": 10,
  "gasPrice": 1
}
```



## Install

```
npm install rpc-check -g
```
