on site token -> buy in on gamble token to nft contract. nft sent to winners wallet

# nft gamble/mint

    buy in to randomize and transfer ownership of 2 nfts from owned nfts

    end user - trade in skins get currency

    currency buy nfts 

    nfts trade out for skin

    server->mint skins and give currency
    server-> give and take currency
    server-> currency to enter gamble contract with nfts as prize
    contract -> entry with currency and wallet adress. winning wallet gets nfts

    contract structs:
        nft metadata: skin price at mint. wear name, and when tradeable
        player data: walletadress and current currenciy
        rngpool: array with nfts in pool

    contract logic: buyin price = avarage price of skins

    handle: enter pool rng, minter reduce currency, minter increase currency, minter add to pool.

# cashout

    trade in nft for skin = send to nft burn
    trade in for currency = send back to gamble contract and add currency

# nftfunc

    getmetadata
    send/transfer ownership
    burn nft

# todo lootcontract

    init()
        DONE nft adress and codehash
        DONE admin adress
        DONE recive nft
    handle()
        DONE recive nft and add to pool
        DONE caluclate pool worth
        DONE use funds to randomize skin
        DONE use adress as prefix
        DONE addFunds()
        DONE removeFunds()
    quary()
        getPoolData
        getFunds(account)


