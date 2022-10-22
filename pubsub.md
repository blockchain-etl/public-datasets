# Public PubSub topics

This is a (possibly incomplete) list of on-chain events that are available in GCP via Pub/Sub. These messages are
derived from crypto nodes that are run in [GCP](https://cloud.google.com). See [system architecture](https://github.com/blockchain-etl/blockchain-etl-architecture) for details.

Each topic is prefixed by `projects/crypto-public-data/topics/` and it's `dataset` field, unless otherwise specified.

For example, for accessing the Ethereum logs topic, append `$DATASET.logs` to get the
full topic name: 

`projects/crypto-public-data/topics/crypto_ethereum.logs`

| Network | Dataset | Blocks | Transactions | Actions | Contracts | Logs | Token Transfers | Tokens | Traces
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- 
| Band | crypto_band | ? | ? | ? | ? | ? | ? | ? | ?
| Bitcoin | crypto_bitcoin | blocks | transactions | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Bitcoin Cash | crypto_bitcoincash | blocks | transactions | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Celo | ? | ? | ? | ? | ? | ? | ? | ? | ?
| Dash | crypto_dash | blocks | transactions | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Dogecoin | crypto_dogecoin | blocks | transactions | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Eos | crypto_eos | blocks | transactions | actions | ❌ | ❌ | ❌ | ❌ | ❌
| Ethereum | crypto_ethereum | blocks | transactions | ❌ | contracts | logs | token_transfers | tokens | traces
| Ethereum 2 | crypto_ethereum2  | ? | ? | ? | ? | ? | ? | ? | ?
| Ethereum Classic | crypto_ethereumclassic  | ? | ? | ? | ? | ? | ? | ? | ?
| Hedera | crypto_hedera | ? | ? | ? | ? | ? | ? | ? | ?
| IoTeX | crypto_iotex | ? | ? | ? | ? | ? | ? | ? | ?
| Litecoin | crypto_litecoin | blocks | transactions | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Polygon | crypto_polygon | ? | ? | ? | ? | ? | ? | ? | ?
| Tezos | crypto_tezos | ? | ? | ? | ? | ? | ? | ? | ?
| Theta | crypto_theta | ? | ? | ? | ? | ? | ? | ? | ?
| XRP | ? | ? | ? | ? | ? | ? | ? | ? | ? | ?
| Zcash | crypto_zcash | blocks | transactions | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Zilliqa | crypto_zilliqa | ? | ? | ? | ? | ? | ? | ? | ?

For examples of how to use pubsub topics, see:
- Blog post: [Live Ethereum and Bitcoin Data in Google BigQuery and Pub/Sub](https://medium.com/google-cloud/live-ethereum-and-bitcoin-data-in-google-bigquery-and-pub-sub-765b71cd57b5)
- Repo: [blockchain-etl/bigquery-to-pubsub](https://github.com/blockchain-etl/bigquery-to-pubsub).
