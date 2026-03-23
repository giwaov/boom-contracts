# Boom Contracts Architecture

## Contract Overview

### boom-pool
The main stacking pool contract that manages delegations and reward distribution.

### boom-nfts
NFT contracts for community and reward NFTs.

### boom-market
Marketplace for trading boom NFTs and other tokens.

## Design Principles

1. **Modularity**: Each contract handles a specific domain
2. **Upgradability**: Key parameters can be updated through governance
3. **Transparency**: All stacking operations are on-chain and verifiable
4. **Security**: Multi-layer authorization for admin functions

## Data Flow

1. User delegates STX to boom-pool
2. Pool operator commits to stacking
3. BTC rewards are earned during the cycle
4. Rewards are distributed proportionally to delegators

## Integration Points

- SIP-010 token standard for reward tokens
- SIP-009 NFT standard for community NFTs
- Stacking PoX contract interactions
