# Digitex Websockets API documentation

This repository contains public specification of Digitex websockets API. Digitex uses Protocol Buffers mechanism to serializing its data.

Current version of .proto file is available in ```/protos``` folder.
You can generate your own client from this protofile. More info about protocol buffers can be found at https://developers.google.com/protocol-buffers.

The proto file is itself well documented. You can also consult autogenerated documentaions that can be found at https://digitexofficial.github.io/ws-api-docs/


## Connection ##

Digitex provides websocket connections to its:
- testnet:  ws.testnet.digitexfutures.com
- mainnet:  ws.mainnet.digitexfutures.com

## Authentication ##

In order to start, you have to register either at
[https://testnet.digitexfutures.com](https://testnet.digitexfutures.com)
for testnet (virtual funds trading) or at 
[https://digitex.io](https://digitex.io) - our mainnet (real money trading).

After registration you need to obtain your trading token in your account.

Direct links to the account page:

- testnet - https://testnet.digitexfutures.com/profile/account
- mainet - https://digitex.io/trade/profile/account

If you have already created your token, you can simply copy it, else click on "Create" in the API section of your account.

You can then use it in the header for authorization using:

```
{"Authorization": "Token YOUR-TOKEN-HERE"}
```


