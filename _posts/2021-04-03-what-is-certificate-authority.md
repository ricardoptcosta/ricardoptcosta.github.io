---
layout: post
author: ricardo
title: What’s the role of a Certificate Authority?
completedness: 30%
order: 2
---

- Setting is: 
    - Alice wants to send message to Bob
    - Alice asks Bob for his public key so that she can encrypt the message with his public key so that only he can can decrypt it
    - Problem is that there can be a man in the middle attack, who will intercept the request and instead return his own public public key to Alice
    - Alice will think she got Bob’s public key and encrypt the message with the thieve’s public key.
- Ensures person who requests the public key gets the correct public key
- The CA, will will sign Bob’s public key (this is done with a human element)
- When we go to a site with https it means that both the messaging is encrypted and that the site is the site I think it is
- In other words:
  - the browser is being told by a CA, which the browser trusts, that the website has sent a honest public key
  - The browser is saying that an entity it trusts  has verified that  this key is the correct key to use when you communicate with the site, say www.sapo.pt.
  - (need to confirm) the key is trusted because it is signed by the CA the browser trusts.
- NOTE: I think this doesn’t work in practice. In practice a session key is generated after the client certificate is verified by the server, the server certificate is verified by the browser, and the browser encrypts its initial messages in order for there to be created and exchanged a session key which will encrypt the session.
