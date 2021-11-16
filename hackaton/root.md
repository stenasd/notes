---
id: gztp3NjFv9UY8WCJUFnas
title: Root
desc: ''
updated: 1636678859722
created: 1636674248381
---

# funktioner
This is the root of your dendron vault. If you decide to publish your entire vault, this will be your landing page. You are free to customize any part of this page except the frontmatter on top. 

    init
        constructor för kontrakt körs en gång i början.

    handle
        tar data från client manipulerar datan och svarar. Kostar gas

    query
        tar medelande och läser det och ger svar kan inte ändra storage 

# parameters

    deps
        get set och remove som ändrar storage på contract
        api: håller adresser?
        querier: funktioner för att querya andra contract
    
    env
        adress som exec kontraktet
        adressen och id till kontr

    msg
        ??? data som skicades

# storage

    keyvalue store med crypterad data och kontracted har bara tillgång till data. Datan är rust struct
    