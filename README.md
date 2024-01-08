# The_Dark_Side_of_NFTs: ALarge-Scale Empirical Study of Wash Trading
source: [https://drive.google.com/drive/folders/1yzLbQURsv-bc9EU4q5BR9cmDmGCodzlY?usp=sharing](https://drive.google.com/drive/folders/1bddfHZgk3BSmDUN0aTAub7mJ-_1_36ff?usp=sharing)
## data
* collectionRaw.zip: the raw data of event sequences of 285 NFT collections with *address inconsistency*, *timestamp error* and *fake events* collected by *OpenSea API*
* collectionPreprocessed.zip: the preprocessed data of event sequences of 285 NFT collections with improved *consisRate*
* ERC-20Price.zip: historical market price of 2,982 ERC-20 tokens collected by *CoinGecko API* 
* pickle_files.zip: 
  * wins_timeWindowInfo.pickle: segmented time windows for event sequences
  * Txn_relatedNormalTransactions.pickle: selected block transactions
  * Txn20_relatedERC20Transactions.pickle: selected ERC-20 transactions
  * real_cir_circlesofTransactionSequences.pickle: details of all cycles in each time window 
  * mr_mergeTransactionSequences.pickle: details of the merged edges 
  * g_graphTransactionSequences.pickle: directed graph constructed by merged edges.
  * fs_validfile.pickle: names of NFT collections
  * flow_relatedNormalTransactions.pickle: details for selected block transactions 
  * flow20_relatedERC20Transactions.pickle: details for selected ERC-20 transactions
  * eth20P_erc20TokenHistoricalPrice.pickle: historical price for ERC-2O tokens
### code
* collection_slug.py: to run collection_slug.py to retrieve event sequences of NFT collections, firstly change the file name with the *collection_slug* of the NFT collection (See example in the following figure / retrieve collecton_slug via *OpenSea API*).  
  `python3 -u collection_slug.py -s start_time -e end_time >collection_slug.log 2>&1`
![image](https://user-images.githubusercontent.com/128060644/228736139-732f90ef-27b4-4f12-b35c-2a0871a9cc2c.png)
* preprocess&overview.py：`python3 preprocess&overview.py`
