## P2SH-P2WSH

- `P2SH-P2WSH` est le sigle pour *Pay to Script Hash - Pay to Witness Script Hash* (en français « payer au hachage du script - payer au témoin du hachage du script »). C’est un modèle de script standard utilisé pour établir des conditions de dépenses sur un UTXO, également connu sous le nom de « Nested SegWit ». `P2SH-P2WSH` a été introduit avec l'implémentation de SegWit en août 2017. Ce script décrit un `P2WSH` enveloppé au sein d'un `P2SH`. Il verrouille des bitcoins sur la base du hachage d'un script. La différence avec `P2WSH` simple est que le script est enveloppé dans le `redeemScript` d'un `P2SH` classique. Ce script a été créé au lancement de SegWit pour faciliter son adoption. Il permet d'utiliser ce nouveau standard, même sur des wallets pas encore compatibles nativement avec SegWit. C'est une sorte de script de transition vers la nouvelle norme. Aujourd'hui, il n'est donc plus très pertinent d'utiliser ce type de scripts SegWit wrappés, puisque la plupart des wallets ont implémenté du SegWit natif. Les adresses `P2SH-P2WSH` sont écrites en utilisant l'encodage `Base58Check` et commencent toujours par `3`, comme n'importe quelle adresse `P2SH`.
