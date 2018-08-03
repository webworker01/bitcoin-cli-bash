# bitcoin-cli-bash

A BASH CLI JSON RPC Interface for Bitcoin and compatible coins

## Requirements

Requires curl and jq (apt-get install jq curl)

## Setup

Simply fill in your rpc user, pass and port in the variables at the beginning of the script to begin using

## Usage

In your terminal run ./bitcoin-cli to see help with a list of available commands

## Altcoin Usage

Just make a copy of the file under whatever name makes sense and fill in the appropriate RPC info. You will find the RPC user and password in the coin's .conf file.  Find the RPC port in chainparams.cpp of the coin's source code.

## Examples

```./bitcoin-cli help getinfo```

```./bitcoin-cli getinfo```

```./bitcoin-cli listunspent 0```


