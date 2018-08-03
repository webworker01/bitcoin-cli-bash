# bitcoin-cli-bash

A BASH CLI JSON RPC Interface for Bitcoin and compatible coins.

Bitcoin already has a bitcoin-cli program so while this script will work with Bitcoin, it's most useful for altcoins that do not have one compiled for their coin, but still have JSON RPC.

## Requirements

Requires curl and jq (apt-get install jq curl)

## Setup

Simply fill in your rpc user, pass and port in the variables at the beginning of the script to begin using. 

You will find the RPC user and password in the coin's .conf file. Find the RPC port in chainparams.cpp of the coin's source code. e.g. Dogecoin RPC port is 22555

## Usage

In your terminal run ./bitcoin-cli to see help with a list of available commands

You can install for system-wide usage by symlinking 

**_WARNING_ - on a shared system any user will now be able to run this command and access your wallet**
```
ln -s /home/user/bitcoin-cli-bash/bitcoin-cli /usr/local/bin/bitcoin-cli
```

Then `bitcoin-cli` will work from any directory without the preceeding `./`

## Altcoin Usage

Just make a copy of the file under whatever name makes sense and fill in the appropriate RPC info. e.g. `dogecoin-cli` 

## Examples

```
./bitcoin-cli help getinfo
```

```
./bitcoin-cli getinfo
```

```
./bitcoin-cli listunspent 0
```

