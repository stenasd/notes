---
id: YvAlVmgs7LC12nT1sBbtM
title: designDoc
desc: ''
updated: 1636679576519
created: 1636679457682
---
# terms
* attribute: metadata for each part token is created from example head=monky body=rabbit and each attribute makes skills available. Attributes + damage against diffrent elements
* moves = moves in pokemon example monkey opens skills throw banana and eat banana
* breeding happens when token lost 3 times
# Game loop
- 2 skills
- winner gets all tokens and losers get breed on them

# design
- text based/image with preselcted skills
- new gens come from breeding

# token 
- attributes that enables and x amount of skills
- 1 attributes from each body part
- each attribute opens list of skills ex tackle and kick.

# etc
- marketplace and trade with token and crypto(scrtcoin or atom)

# psoudo gameplay
    server
        server will do matchmaking
    init 
        put up for arena with private nft data.
    handle
        do game calc and transfer ownership to loser
        use nft metadata for calc winner or loser. change storage to winner.
    quary
        actions that detrmined winner

# psoudo minting
    init setup all available nft that can get minted
    handle
        randomise from list of nft and give out 3 and remove from list
# psudo breed
    init 
        2 tokens enter
    handle
        fee = 1/3 minting price
        2 tokens enter 3 out with minted child random atributes between parrents
# psudo reroll
    init
        1 token
    handle
        1 token enter
        1 token exit with rerolled moves
