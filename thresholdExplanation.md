# Our explanation for the threshold:  
Choosing different values for the key parameters in our algorithm produces different results. We actually provide a value reference while guaranteeing the correctness of the results and allowing researchers to adjust them according to datasets of various sizes. See how we determine the value from here.
## Fig 1: Distribution of the number of round-trip trading behaviors with different thresholds from 4 to 100
*Explanation: More false positive cases are identified when the threshold is at a low level. If it was set in the interval from 25 to 100, the number of round-trip trading behaviors remains almost the same. In other words, 100 is a strict threshold.*
![image](https://github.com/NFTWashTrading/The_Dark_Side_of_NFTs/assets/128060644/ef79fe69-1018-4410-a6b4-8677526f604a)
## Fig 2: Distribution of the number of ERC-20 token transfer behaviors within one hour before and after the NFT sale events
*Explanation: The number of ERC-20 transfers experience multiple fluctuations over a ten-hour period. To identify ERC-20 transfers associated with NFT transactions, we select only the first fluctuation, i.e., around the first 80 minutes.*
![image](https://github.com/NFTWashTrading/The_Dark_Side_of_NFTs/assets/128060644/2fc8f361-99c7-4cff-a0ee-f617fd568ce7)
## Fig 3: Distribution of the number of ETH transfer behaviors within one hour before and after the NFT sale events
*Explanation: The number of ETH transfers experiences a steep rise and fall within 20 minutes from the sale events, after which it stays at a low level with a downward trend. It indicates that ETH transfers within 20 minutes correlate more strongly with the sale event.*
![image](https://github.com/NFTWashTrading/The_Dark_Side_of_NFTs/assets/128060644/e263dfac-c657-4304-8c9c-779afcb9342a)
