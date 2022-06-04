# TruffleRinkeby
Rinkebyにデプロイするための開発用リポジトリになります。

## Rinkebyにデプロイする方法

 `truffle console --network rinkeby`
 `migrate`

 うまくいけばコンソールに次の様に出力される。

 ```cmd
 1_initial_migration.js
======================

   Deploying 'Migrations'
   ----------------------
   > transaction hash:    0x03cfe0c0c6b697119b3ec7b660f4c97fa539cbddbc1530482d00524443e33f34
   > Blocks: 1            Seconds: 13
   > contract address:    0xA5C193EfA151C1266A8bc8aA285f44DE4d45FA6d
   > block number:        10793448
   > block timestamp:     1654342567
   > account:             0x51908F598A5e0d8F1A3bAbFa6DF76F9704daD072
   > balance:             155.576824743621387904
   > gas used:            130474 (0x1fdaa)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00260948 ETH

   Pausing for 2 confirmations...
   ------------------------------
   > confirmation number: 1 (block: 10793449)
   > confirmation number: 2 (block: 10793450)

   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:          0.00260948 ETH


2_deploy_contracts.js
=====================

   Deploying 'ConvertLib'
   ----------------------
   > transaction hash:    0xdf973b5c327f171e4d272d394a35ecf5c3972509abe5666b3394c348b32300d3
   > Blocks: 0            Seconds: 9
   > contract address:    0x39466Be45A95D44201924B04aB59985aFb427249
   > block number:        10793452
   > block timestamp:     1654342627
   > account:             0x51908F598A5e0d8F1A3bAbFa6DF76F9704daD072
   > balance:             155.574135903621387904
   > gas used:            88776 (0x15ac8)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00177552 ETH

   Pausing for 2 confirmations...
   ------------------------------
   > confirmation number: 1 (block: 10793453)
   > confirmation number: 2 (block: 10793454)

   Linking
   -------
   * Contract: MetaCoin <--> Library: ConvertLib (at address: 0x39466Be45A95D44201924B04aB59985aFb427249)

   Deploying 'MetaCoin'
   --------------------
   > transaction hash:    0xa67de5095ea8d89a1d221a2da7b24bee374fe45bca88e16e1332fef008a39ec5
   > Blocks: 1            Seconds: 9
   > contract address:    0xdc241458C483BDa3fB06d22B245Ca6823c0f4b8b
   > block number:        10793455
   > block timestamp:     1654342672
   > account:             0x51908F598A5e0d8F1A3bAbFa6DF76F9704daD072
   > balance:             155.570041723621387904
   > gas used:            204709 (0x31fa5)
   > gas price:           20 gwei
   > value sent:          0 ETH
   > total cost:          0.00409418 ETH

   Pausing for 2 confirmations...
   ------------------------------
   > confirmation number: 1 (block: 10793456)
   > confirmation number: 2 (block: 10793457)

   > Saving migration to chain.
   > Saving artifacts
   -------------------------------------
   > Total cost:           0.0058697 ETH


Summary
=======
> Total deployments:   3
> Final cost:          0.00847918 ETH
 ```

### デプロイしたコントラクトの情報

Rinkeby上のアドレス

|コントラクト名|アドレス|
|----|-----|
|FundraiserFactory|<a href="https://rinkeby.etherscan.io/address/0x0CFAA30F17A950BA1a24504e6c4D2BafCBdB32bf">0x0CFAA30F17A950BA1a24504e6c4D2BafCBdB32bf</a>|
|NFTFactory|<a href="https://rinkeby.etherscan.io/address/0x1B55d7D92eF282A29a24Aa10dFA1bED0aBAd681a">0x1B55d7D92eF282A29a24Aa10dFA1bED0aBAd681a</a>|
|MyTokenFactory|<a href="https://rinkeby.etherscan.io/address/0xA7636EF9cA7260acD6d1B9226686c8a06cC55EaE">0xA7636EF9cA7260acD6d1B9226686c8a06cC55EaE</a>|
|DEX|<a href="https://etherscan.io/address/0xbCc9468062C427E937bc38b100F5821728223068">0xbCc9468062C427E937bc38b100F5821728223068</a>|