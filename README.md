# preferred_wifi
Preferred wifi reconnect for Linux

## Summary

This script will look for a preferred wifi network. If the the network is available *and* the computer is not connected to it then it will attempt to connect to it (likely disconnecting the current wifi connection in the process).

It is meant to be called periodically by cron.

## Usage

```
preferred_wifi CONNECTION [-v]
```

 - `CONNECTION` : The NetworkManager connection name for the preferred wifi network
 - `-v` : Verbose
 
## Motivation

NetworkManager can connect automatically to wifi networks. However it does not switch to a new wifi network if it is already connected to one.

## Requirements

NetworkManager's `nmcli`
