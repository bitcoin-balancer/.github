[< Back](../../../README.md#position-management)

# Strategy

Balancer gives users full control over their trading strategy and budget allocation through a simple, user-friendly form available in the GUI.

The trading strategy consists of the following parameters:

## Increase

### Amount

The amount of quote asset (USDT) that will be used to open/increase positions.

### Gain requirement%

The position must be at a loss of at least "Gain requirement%" to be increasable.

For example, say the "Gain requirement%" is set at -10%, and a position opens at $1,000/BTC. For it to be increasable, the price of BTC must drop to at least $900.

Setting 0 disables this functionality. Meaning that the position can be increased on every reversal event regardless of the gain state.

### Idle duration

The number of hours Balancer will wait before being able to increase the position again.

For example, if the "Idle duration" is set to 24 hours and a position is opened on Monday at 2 pm, Balancer won't be able to increase the position until Tuesday at 2 pm regardless of the state of the market.

### Idle mode

Balancer's Idle mode governs the waiting period before a position can be increased. Two modes are supported:

- **Incremental:** the waiting period is "Idle duration" multiplied by the number of previous increases. For example, with "Idle duration" set to 24 hours and 5 previous increases, the wait time becomes 120 hours (24 \* 5).

- **Fixed:** the waiting period is always "Idle duration", regardless of the number of previous increases.

<br/>

## Decrease

Balancer uses **five** distinct decrease levels that activate once the position's profit meets the specified gain threshold. The higher the level, the larger and more frequent the reductions.

Each level has the following properties:

### Gain requirement%

The gain required for the level to be active.

### Percentage

The percentage of the position amount that will be decreased when the level is active and conditions apply.

### Frequency

The number of minutes in which the interval will continue to decrease the position (as long as the conditions are met).
