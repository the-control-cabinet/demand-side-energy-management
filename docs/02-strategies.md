# 02 Strategies

[← Back to README](../README.md)

1. **Cheapest window:** schedule each flexible load into the lowest-price slots that still meet its constraint.
2. **Cleanest window:** the same, ranked by carbon intensity (a selectable objective, or a weighted blend).
3. **Peak-demand limiting:** if import exceeds a threshold (e.g. 7 kW) for 2 min, reduce or defer loads in priority order (EV first; never heating safety or DHW minimums), restoring with hysteresis.
4. **Event response:** during a supplier event, pause flexible loads and log the delivered reduction.
5. **Fail-safe:** if prices or data are unavailable, revert each device to its own schedule.
