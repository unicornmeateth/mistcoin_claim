# 🦄 Unicorn Meat Mistcoin Claim

Merkle tree data for Unicorn Meat token claim for Mistcoin holders on Ethereum L1.

## 📋 Claim Data

- **Total Claims**: 1,200 addresses
- **Total Allocated**: 2,398,896 tokens
- **Merkle Root**: `0x58eb938871a597c9fa119b622519fb716c7c8e7a9159ed7d1dee4ee0ea4d8aa3`
- **Contract**: [0x1eD74EaACE8a96A79BCa9099696723134c0F6751](https://etherscan.io/address/0x1eD74EaACE8a96A79BCa9099696723134c0F6751)

## 🔍 How to Find Your Claim

1. **Search for your address** in `merkle-data-mistcoin.json`
2. **Find your entry** with your address, amount, and proof array
3. **Use the amount and proof** to claim your tokens

Example entry:
```json
{
  "address": "0xf07a2439296e07bc4320af924e655a01fb69d89c",
  "amount": 20000,
  "proof": ["0xb312138c...", "0x9e3ce829...", ...]
}
```

## 🚀 How to Claim

### Option 1: Etherscan
1. Go to the [contract on Etherscan](https://etherscan.io/address/0x1eD74EaACE8a96A79BCa9099696723134c0F6751)
2. Connect your wallet
3. Use the "Write Contract" tab
4. Call `claim` with your amount and proof array

### Option 2: Use the Unicorn Meat Website
Visit the [Unicorn Meat](https://www.unicornmeateth.com) and find the claim section.

## 🔒 Security

- ✅ **Safe to share**: Only contains public addresses and amounts
- ✅ **On-chain verification**: Claims verified using Merkle root
- ✅ **Any wallet**: Claim from any wallet (doesn't need to be your Mistcoin wallet)
- ✅ **Cold wallet friendly**: Perfect for users with tokens in cold storage

## 📊 Data Structure

The JSON file contains:
- `merkleRoot`: The root hash used by the contract
- `totalAllocated`: Total tokens allocated for claims
- `totalClaims`: Number of eligible addresses
- `claims`: Array of all claim data with addresses, amounts, and proofs

## ❓ FAQ

**Q: Can I claim from a different wallet?**
A: Yes! You can claim from any wallet using your address and proof.

**Q: What if I have tokens in a cold wallet?**
A: Perfect! Claim from any wallet (hot, hardware, etc.) using your proof.

**Q: How do I know my allocation is correct?**
A: Check the JSON file for your address. The amount shown is your exact allocation.

**Q: Is this data safe to share?**
A: Yes! This only contains public information and Merkle proofs designed to be shared.

---

**Note**: This claim is for Mistcoin holders on Ethereum L1. Make sure you're interacting with the correct contract address. 