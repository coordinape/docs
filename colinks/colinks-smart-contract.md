# CoLinks Smart Contract

The CoLinks social-fi smart contract is a fork of Friend.Tech’s landmark design. However, we do a few things differently. Please refer to our Terms of Service to understand viable use of the CoLinks smart contract.

### **CoLinks is deployed on Optimism Mainnet**

* Contract Address is[ here](https://optimistic.etherscan.io/address/0x7154cA7E4C756E06151aefA2D765404950FA0EE1).

### **Softer bonding curve**

* We have optimized our bonding curve for people to accumulate larger collections of Links, by making the curve less steep than Friend.Tech.&#x20;
* This allows more Link connections to be made before prices become prohibitive.

### Familiar Fees

* Like Friend Tech, the Link subject and Coordinape Foundation will each take 5% of the buy or sell price as an added fee with each transaction.

### Additional Base Fee Split

* To compensate for the softer curve, Coordinape and the Link offerer will split a small flat fee on each buy and sell. This fee is currently set to .000042 ETH
* This fee is applied in full on all Buys, but ramps up on Sells to allow for sellers to recapture value on sells below the Base Fee itself.

### Contract Management

* Just like the Friend Tech contract, OP ETH that is placed in escrow in the contract is not accessible to anyone other than Link holders. Even the contract owner multisig cannot remove it.
* Contract owner (multisig) can change fee values and protocol fee destination.
* There are reasonable maximums set on the fees in the contract, to prevent fees that are too high.
