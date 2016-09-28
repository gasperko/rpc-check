# RPC Check

[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://github.com/sebs/rpc-check/blob/master/LICENSE)

[![Release](http://img.shields.io/github/release/sebs/rpc-check.svg?style=flat-square)](https://github.com/sebs/rpc-check/releases)

Checks for JSON RPC nodes of ethereum nodes and displays basic statistics

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
