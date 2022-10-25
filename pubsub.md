# Public PubSub topics

This is a (possibly incomplete) list of on-chain events that are available in GCP via Pub/Sub. These messages are
derived from crypto nodes that are run in [GCP](https://cloud.google.com). See [system architecture](https://github.com/blockchain-etl/blockchain-etl-architecture) for details.

Each topic is prefixed by `projects/` and it's `project` and `dataset` fields, unless otherwise specified.

For example, for accessing the Ethereum logs topic, append `$PROJECT/topics/$DATASET.logs` to get the
full topic name: 

`projects/crypto-public-data/topics/crypto_ethereum.logs`

| Network | Project | Dataset | blocks | transactions | logs | contracts | token_transfers | tokens | traces | events | messages | oracle_requests | block_events | transaction_logs | actions
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | ---
| Band         | public-data-finance | crypto_band        | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ✅ | ✅ | ✅ | ✅ | ❌ | ❌
| Bitcoin      | crypto-public-data  | crypto_bitcoin     | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Bitcoin Cash | crypto-public-data  | crypto_bitcoincash | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Celo         | nansen-public-data  | crypto_celo        | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔
| Dash         | crypto-public-data  | crypto_dash        | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Dogecoin     | crypto-public-data  | crypto_dogecoin    | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Eos          | crypto-public-data  | crypto_eos         | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Ethereum     | crypto-public-data  | crypto_ethereum    | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Ethereum 2   |                  ?  | crypto_ethereum2   | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Ethereum Classic |              ?  | crypto_ethereumclassic  | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Fantom       | nansen-public-data  | crypto_fantom      | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔
| Hedera       |                  ?  | crypto_hedera      | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔
| IoTeX        | public-data-finance | crypto_iotex       | ✅ | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ | ❌
| Litecoin     | crypto-public-data  | crypto_litecoin    | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Polygon      | public-data-finance | crypto_polygon     | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Tezos        |                  ?  | crypto_tezos       | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔
| Theta        |                  ?  | crypto_theta       | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔
| XRP          |                  ?  | ?                  | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔
| Zcash        | crypto-public-data  | crypto_zcash       | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌
| Zilliqa      |                  ?  | crypto_zilliqa     | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔ | ❔

For examples of how to use pubsub topics, see:
- Blog post: [Live Ethereum and Bitcoin Data in Google BigQuery and Pub/Sub](https://medium.com/google-cloud/live-ethereum-and-bitcoin-data-in-google-bigquery-and-pub-sub-765b71cd57b5)
- Repo: [blockchain-etl/bigquery-to-pubsub](https://github.com/blockchain-etl/bigquery-to-pubsub).
