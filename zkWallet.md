# Simplicy - zkWallet Social Recovery
Simplicy zkWallet is a social recovery smart contract wallet using zk-SNARKS to restore a user's access to their smart contract wallet, without revealing any information of the user's and **guardians**.

## Wallet design
zk-SocialRecoveryWallet wallet design:
- **Simplicity**: average users (non crypto users) should be able to create and use the wallet.
- **Frictionless**: most normal activities should not require much more effort than they do in regular wallet (e.g Metamask).
- **Privacy**: never send user data onchain. Must operate under the General Data Protection Regulation (GDPR).
- **Anonymous**: an account is a fresh cryptographic hash, not tied to existing systems or real-world identity. Derived paths support multiple public keys to protect privacy.

### Security
- **No single point of failure**: there is no single thing which, if stolen, can give an attacker access to user's funds, or if lost, can deny user's access to their funds.
- **Keyless**: no key's will be stored in a client web- or mobile app. 
- **Sufficient**
- **Self-Sovereign**: user's have full custody and self control of their wallet.
- **Verifieable**: trusted are only open source and hardened cryptography

### Smart contract designs
- **Open source**: community driven. Reduce the risk of vulnerabilities by using standard, tested, community-reviewed code.
- **Diamond standard upgradeable**: modular approach, simple, robust facets code.
- **Diamond storage pattern**: seperate business logics from the storage. 

## Documentation
<https://github.com/zkWallet/zkWallet-docs/blob/main/README.md>

# Sources
- [Why we need wide adoption of social recovery wallets](https://vitalik.ca/general/2021/01/11/recovery.html)
- [EIP-2535: Diamonds, Multi-Facet Proxy](https://eips.ethereum.org/EIPS/eip-2535)
- [Diamond storage pattern](https://medium.com/1milliondevs/new-storage-layout-for-proxy-contracts-and-diamonds-98d01d0eadb)
