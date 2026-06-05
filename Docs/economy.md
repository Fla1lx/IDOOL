# IDOOL Economy Draft

## Main Resource

Money is the main resource in the MVP. The player earns money from completed repairs and spends it on workshop upgrades.

The early economy should keep decisions frequent, readable, and low-pressure. The player should see progress every few repairs.

## Repair Types

| Repair Type | Duration | Base Reward | Purpose |
| --- | ---: | ---: | --- |
| Tire check | 10 sec | 15 | Fast first action and tutorial-friendly repair. |
| Oil change | 20 sec | 35 | Baseline job for early progression. |
| Brake service | 35 sec | 70 | Slower job with a stronger reward. |
| Engine tune-up | 60 sec | 140 | Early long job that encourages upgrades. |

## Repair Rewards

Rewards are paid when the repair timer completes. Upgrade bonuses can multiply the final reward or add a flat bonus.

Initial formula draft:

```text
final_reward = base_reward * reward_multiplier
```

For the MVP, `reward_multiplier` can start at `1.0` and increase through workshop upgrades.

## Workshop Upgrades

| Upgrade | Effect | Starting Price | Price Growth |
| --- | --- | ---: | ---: |
| Better tools | Reduces repair duration by 10% per level. | 75 | x1.6 |
| Service quality | Increases repair rewards by 15% per level. | 100 | x1.7 |
| Parking slots | Increases queue capacity by 1 per level. | 150 | x2.0 |

Upgrade prices should be rounded to clean values for readability.

## First 10-15 Minutes Balance Example

Starting state:

- Money: 0
- Queue capacity: 2 cars
- Repair bay count: 1
- Repair speed multiplier: 1.0
- Reward multiplier: 1.0

Expected early flow:

| Minute | Target Experience |
| ---: | --- |
| 0-1 | Complete one tire check and understand the repair timer. |
| 1-3 | Complete oil changes and tire checks, reaching 75-100 money. |
| 3-5 | Buy the first tool or reward upgrade. Repairs now feel slightly better. |
| 5-8 | Unlock enough income to choose between speed, reward, or queue capacity. |
| 8-12 | Complete at least one brake service and one engine tune-up. |
| 12-15 | Own 2-4 total upgrades and feel the workshop becoming more efficient. |

Draft target by minute 15:

- Total earned money: 500-800
- Upgrade count: 2-4
- Average repair duration after upgrades: 10-20% faster than start
- Queue capacity: 2-3 cars
