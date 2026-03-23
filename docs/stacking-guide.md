# Stacking with Boom Contracts

## Overview
Boom Pool allows STX holders to participate in Stacking (Proof of Transfer) with smaller amounts by pooling funds.

## How Stacking Works on Stacks

1. Lock STX tokens for a number of cycles
2. Earn BTC rewards from miners
3. Tokens are unlocked after the stacking period

## Using Boom Pool

### Delegate STX
```clarity
(contract-call? .boom-pool delegate-stx u1000000)
```

### Check Stacking Status
```clarity
(contract-call? .boom-pool get-stacker-info tx-sender)
```

### Withdraw After Period
```clarity
(contract-call? .boom-pool withdraw-stx)
```

## Minimum Requirements
- Minimum STX amount varies by cycle
- Delegation must be done before the cycle starts
- Rewards are distributed proportionally

## Risk Considerations
- STX are locked during the stacking period
- Smart contract risk
- BTC reward variability based on miner activity
