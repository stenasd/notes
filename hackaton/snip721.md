---
id: WqwmGkfVSdfOM9qZWvJul
title: Snip721
desc: ''
updated: 1636707067425
created: 1636678849002
---

# snip 721

Baserad på erc 721 och cw 721. 

# terms

- **msg** on chain reference triggas av att skicka en trans och on chain svar. Behöver auth

- **Query** off chain data som noden har lokalt 

- **Cosmos Message Sender** konto som är hittad under sender i cosmos sdk message och den som signar och behöver auth i **msg**

# minting 
- bara tillåtna adresser kan minta en token
- **metadata** public och private private kan ägeren över token se.

# seal
- Gömmer metadata tills den är unwraped
