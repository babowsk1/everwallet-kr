# Types of wallet

EVER Wallet supports the creation of several types of wallets, which differ in the specifics of their work:

**SafeMultisig** - formally verified Multisig wallet. \
**SafeMultisig24** - with a SafeMultisig wallet custodian confirmations take up to 1 hour, with a SafeMultisig24 it will take up to 24 hours. If the required number of signatures is not reached by the time limit, the transaction will be nullified. \
**SetCodeMultisigWallet** - Multisig wallet with the possibility to change codes and custodians. **BridgeMultisigWallet** - this kind of wallet differs from SafeMultisig because it does not have payload limits.&#x20;

{% hint style="info" %}
If you want to use a multisig wallet with 3 or more custodians on [FlatQube ](broken-reference)and [Octus Bridge](https://docs.octusbridge.io/), be sure to use **BridgeMultisigWallet** type!
{% endhint %}

**Surf** - Technically, this kind of wallet is the same as SetCodeMultisig. You should use this kind of wallet to import your Ever Surf wallet. \
**WalletV3** - this is a small and simple contract that allows you to deploy your wallet at the same time as you make a transfer and has a 24-word seed phrase.
