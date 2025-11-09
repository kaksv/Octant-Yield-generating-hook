## OctantVaultHook – Powering Public Goods Through Intelligent Liquidity**

**Overview**
In traditional AMMs, liquidity providers (LPs) earn trading fees—but those fees rarely serve broader ecosystem goals. The OctantVaultHook reimagines this model:

- A dynamic fee (0.0%–10%) is applied based on swap size.

- A portion of generated fees flows directly into an Octant Vault to fund verified public goods.

- Remaining fees incentivize LPs and reinforce pool depth.

- Smart range optimization ensures LP capital stays productive.

- Time-based withdrawal penalties discourage short-term speculation and protect pool stability.

This creates a self-sustaining loop: more liquidity → more swaps → more fees → more public goods funding → stronger ecosystem → more demand for liquidity.

## 💡 Core Mechanics
_1. Dynamic Fee Structure_
|  Swap magnitude  | Fee Tier |
| Very Large       | 10.0%    |
| Large            | 5.0%     |
| Medium           | 2.5%     |
| Small            | 1.0%.    |
| Tiny             | 0.0%     |

_2. Fee Allocation_

- 40% → Octant Vault (funds public goods)

- 50% → LPs (as yield incentive)

- 10% → Pool Reserves (to deepen liquidity)

_3. Early Withdrawal Slash_
To prevent liquidity churn and ensure pool stability.

_4. Zero-Fee Fallback_
If no fees are generated in 24 hours, a minimal 0.003% of LP principal is redirected to the Octant Vault—ensuring continuous public goods funding even in low-activity periods.

_5. Auto-Range Optimization (“Maximize Yield” Mode)_
LPs can opt into auto-range rebalancing:

- After each swap, the hook checks if the LP’s position is in-range.
- If out-of-range, the hook automatically redeployes liquidity into a new optimal price range on behalf of the LP.
- Uses on-chain oracles or recent price data to determine ideal ranges.
- Minimizes idle capital and maximizes fee capture.

## How to test the hook

1. Clone the github repository and use foundry to install the dependences, configure remappings.txt file and test using the provided scripts or run custom tests, then deploy the hook on the Ethereum mainnet. The vault linked to in the hook is the Spark Eth vault on the Ethereum Mainnet.




