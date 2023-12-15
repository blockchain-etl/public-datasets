# Public Blockchain Datasets

| Network | BigQuery | Lag | PubSub | Node repo(s) | Indexer repo(s)
| --- | --- | --- | --- | --- | --- 
| Band | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_band&p=public-data-finance) ([Examples](https://console.cloud.google.com/marketplace/product/public-data-finance/crypto-band-dataset)) | 0 | [💧](pubsub.md) | [band-kubernetes](https://github.com/blockchain-etl/band-kubernetes) | [band-etl](https://github.com/blockchain-etl/band-etl)
| Bitcoin | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_bitcoin&p=bigquery-public-data) ([Examples](https://console.cloud.google.com/marketplace/product/bitcoin/crypto-bitcoin)) | 3 | [💧](pubsub.md) | [docker-bitcoind](https://github.com/blockchain-etl/docker-bitcoind) | [bitcoin-etl](https://github.com/blockchain-etl/bitcoin-etl), [bitcoin-etl-airflow](https://github.com/blockchain-etl/bitcoin-etl-airflow), [bitcoin-etl-airflow-neo4j](https://github.com/blockchain-etl/bitcoin-etl-airflow-neo4j), [bitcoin-etl-streaming](https://github.com/blockchain-etl/bitcoin-etl-streaming)
| Bitcoin Cash | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_bitcoin_cash&p=bigquery-public-data) ([Examples](https://console.cloud.google.com/marketplace/product/bitcoin-cash/crypto-bitcoin-cash))| 6 | [💧](pubsub.md) | [docker-bitcoin-cashd](https://github.com/blockchain-etl/docker-bitcoincashd) | see Bitcoin
| Celo | [🔍](https://console.cloud.google.com/bigquery?page=table&d=crypto_celo&p=nansen-public-data&t=transactions) | 10 | [💧](pubsub.md) | ? | [celo-etl](https://github.com/nansen-ai/celo-etl)
| Dash | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_dash&p=bigquery-public-data) ([Examples](https://console.cloud.google.com/marketplace/product/dash/crypto-dash)) | 24 | [💧](pubsub.md) | [docker-dashd](https://github.com/blockchain-etl/docker-dashd) | see Bitcoin
| Dogecoin | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_dogecoin&p=bigquery-public-data) ([Examples](https://console.cloud.google.com/marketplace/product/dogecoin/crypto-dogecoin)) | 60 | [💧](pubsub.md) | [docker-dogecoind](https://github.com/blockchain-etl/docker-dogecoind) | see Bitcoin
| Ethereum | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_ethereum&p=bigquery-public-data) ([Examples](https://console.cloud.google.com/marketplace/product/ethereum/crypto-ethereum-blockchain)) | 18 | [💧](pubsub.md) | ? | [ethereum-etl](https://github.com/blockchain-etl/ethereum-etl), [ethereum-etl-airflow](https://github.com/blockchain-etl/ethereum-etl-airflow), [ethereum-etl-neo4j](https://github.com/blockchain-etl/ethereum-etl-neo4j), [ethereum-etl-postgres](https://github.com/blockchain-etl/ethereum-etl-postgres)
| Ethereum 2 | [🔍](https://console.cloud.google.com/bigquery?page=table&t=beacon_blocks&d=crypto_ethereum2&p=public-data-finance) | ? | ❌ | ? | [ethereum2-etl](https://github.com/blockchain-etl/ethereum2-etl), [ethereum2-etl-airflow](ethereum2-etl-airflow)
| Ethereum Classic| [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_ethereum_classic&p=bigquery-public-data) ([Examples](https://console.cloud.google.com/marketplace/product/ethereum-classic/crypto-ethereum-classic)) | ? | ❌ | see Ethereum | see Ethereum
| Fantom | [🔍](https://console.cloud.google.com/bigquery?page=table&d=crypto_fantom&p=nansen-public-data&t=transactions) | ? | [💧](pubsub.md) | ? | ?
| Hedera Hashgraph | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=mainnet&p=hedera-etl) | ? | ? | ? | [hedera-etl](https://github.com/blockchain-etl/hedera-etl) | ? | ?
| IoTeX | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_iotex&p=public-data-finance) ([Examples](https://console.cloud.google.com/marketplace/product/public-data-finance/crypto-iotex-dataset)) | 10 | [💧](pubsub.md) | [iotex-kubernetes](https://github.com/blockchain-etl/iotex-kubernetes) | [iotex-etl](https://github.com/blockchain-etl/iotex-etl)
| Litecoin | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_litecoin&p=bigquery-public-data) ([Examples](https://console.cloud.google.com/marketplace/product/litecoin/crypto-litecoin)) | 12 | [💧](pubsub.md) | [docker-litecoind](https://github.com/blockchain-etl/docker-litecoind) | see Bitcoin 
| MultiversX | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_multiversx_mainnet_eu&p=bigquery-public-data) ([Examples](https://console.cloud.google.com/marketplace/product/bigquery-public-data/blockchain-analytics-multiversx-mainnet-eu)) | ? | ❌ | [mx-chain-go](https://github.com/multiversx/mx-chain-go) | [multiversx-etl](https://github.com/multiversx/multiversx-etl)
| Polygon | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_polygon&p=public-data-finance) ([Examples](https://console.cloud.google.com/marketplace/product/public-data-finance/crypto-polygon-dataset)) | 80 | [💧](pubsub.md) | ? | [polygon-etl](https://github.com/blockchain-etl/polygon-etl)
| Tezos | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_tezos&p=public-data-finance) ([Examples](https://console.cloud.google.com/marketplace/product/public-data-finance/crypto-tezos-dataset)) | ? | ? | [tezos-kubernetes](https://github.com/blockchain-etl/tezos-kubernetes) | [tezos-etl](https://github.com/blockchain-etl/tezos-etl), [tezos-etl-airflow](https://github.com/blockchain-etl/tezos-etl-airflow)
| Theta | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_theta&p=public-data-finance) ([Examples](https://console.cloud.google.com/marketplace/product/public-data-finance/crypto-theta-dataset)) | ? | ? | ? | [theta-etl](https://github.com/blockchain-etl/theta-etl)
| XRP | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=fullhistory&p=xrpledgerdata) | ? | ? | ? | [fetch-xrpl-transactions](https://github.com/WietseWind/fetch-xrpl-transactions)
| Zcash | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_zcash&p=bigquery-public-data) ([Examples](https://console.cloud.google.com/marketplace/product/zcash/crypto-zcash)) | 24 | [💧](pubsub.md) | [docker-zcashd](https://github.com/blockchain-etl/docker-zcashd) | see Bitcoin 
| Zilliqa | [🔍](https://console.cloud.google.com/bigquery?page=table&t=transactions&d=crypto_zilliqa&p=public-data-finance) ([Examples](https://console.cloud.google.com/marketplace/product/public-data-finance/crypto-zilliqa-dataset)) | ? | ? | ? | [zilliqa-etl](https://github.com/blockchain-etl/zilliqa-etl)

# Planning / Building
| Network | BigQuery | Lag | PubSub | Node repo(s) | Indexer repo(s) | Notes
| --- | --- | --- | --- | --- | --- | ---
| Algorand  | ⏳ | ? | ⏳ | ? | ? | Needs help
| Aptos     | ⏳ | ? | ⏳ | ? | ? | Needs help
| Arbitrum  | ⏳ | ? | ⏳ | ? | ? | Needs help
| Avalanche | ⏳ | ? | ⏳ | ? | ? | Needs help
| BNB Chain | ⏳ | ? | ⏳ | ? | ? | Needs help
| Cronos    | ⏳ | ? | ⏳ | ? | ? | Needs help
| Eos       | ❌ | ? | ❌ | ? | [eos-etl](https://github.com/blockchain-etl/eos-etl), [eos-etl-airflow](https://github.com/blockchain-etl/eos-etl-airflow) | Needs help
| Icon      | ❌ | ? | ❌ | ? | [icon-etl](https://github.com/blockchain-etl/icon-etl), [icon-etl-airflow](https://github.com/blockchain-etl/icon-etl-airflow) | Needs help
| Klaytn    | 👷 | ? | 👷 | ? | [klaytn-etl](https://github.com/klaytn/klaytn-etl) | In progress
| Optimism  | ⏳ | ? | ⏳ | ? | ? | Needs help
| Solana    | 👷 | ? | 👷 | ? | [solana-etl](https://github.com/blockchain-etl/solana-etl) | In progress
| Sui       | ⏳ | ? | ⏳ | ? | ? | Needs help
