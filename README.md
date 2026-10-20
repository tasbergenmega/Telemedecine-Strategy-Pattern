## Assignment 5: Strategy Pattern

### Table of Classes
| Class | Responsibility |
|---|---|
| `PricingStrategy` | Declares the algorithm contract for calculating price. |
| `StandardPricing` | Calculates standard price for regular patients. |
| `VipPricing` | Calculates price with VIP surcharge. |
| `NightPricing` | Calculates price with night time multiplier. |
| `DoctorMatchingStrategy` | Declares the algorithm contract for doctor selection. |
| `PricingContext` | Holds and delegates to the selected pricing strategy. |
| `PricingSelector` | Chooses a pricing strategy automatically based on demand. |

### Why Strategy and not State or Template Method?
We use Strategy because we have multiple interchangeable algorithms (pricing, matching) that must be selected at runtime. State is for changing behavior based on internal state transitions, and Template Method defines the skeleton of an algorithm, letting subclasses override steps. Here, the client explicitly requests a specific algorithm, and we can swap it dynamically without changing the context.

### Git Commits
*   **Commit 1 (Bad way):** [Insert link to commit 1]
*   **Commit 2 (Refactored):** [Insert link to commit 2]
