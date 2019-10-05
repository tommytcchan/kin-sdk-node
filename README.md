# Kin SDK for Node

Kin SDK for Node is meant to be used as a back-end service. It can perform actions for your client apps (iOS, Android, etc.) 
and also operate as a server for you to build services on top of the Kin blockchain. 
For example, the SDK can communicate with the Kin Blockchain on behalf of the client to create accounts and whitelist transactions. 
It can also monitor blockchain transactions so that you can implement broader services. 
It is up to you how to integrate the SDK in your overall architecture and how to manage your server.

# Installation Notes
If you encounter an error while performing `npm install` with the error below, then you will need to downgrade you Node version to 11. Node >= 12 removed some functions that the `ed25519` library

```
../src/ed25519.cc:19:89: error: no matching member function for call to 'ToObject'
        if ((info.Length() < 1) || (!Buffer::HasInstance(info[0])) || (Buffer::Length(info[0]->ToObject()) != 32)) {
```

<a href="https://kinecosystem.github.io/kin-website-docs/docs/documentation/nodejs-sdk"><img src="https://partners.kinecosystem.com/img/documentation-button2x.png" width=300 height=84 alt="Documentation"/></a>
