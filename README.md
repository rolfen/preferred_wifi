# preferred_wifi
Preferred wifi reconnect for Linux

## Summary

This script will look for a preferred wifi network. If the the network is available *and* the computer is not connected to it then it will attempt to connect to it (likely disconnecting the current wifi connection in the process).

It is meant to be called periodically by cron.

## Usage

```
preferred_wifi CONNECTION [-v]
```

 - `CONNECTION` : The NetworkManager connection name for the preferred network
 - `-v` : Verbose
 
 ## Motivation

NetworkManager can connecte automatically to wifi networks. However it will not reconnect to a different wifi network if it is already connected to one.
