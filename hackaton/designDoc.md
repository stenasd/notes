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
* token become breedable when it has lost 3+ times and can breed with anytoken
# Game loop
- 2 skills loop in order of "counter" power and loops 10 times and most hp wins
- winner gets all tokens and lost token get breed stack on them

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
    init 
        put up for arena with private nft data. sets player 1 to caller
    handle
        join() a tokens joins and battle plays out
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
# psudo token
    can change nick memo and current moves
        nick= name that user given him
        memo= msg on token when viewed
        moves= currently selected moves
        owned moves and quality on moves

