# 01 Signals and loads

[← Back to README](../README.md)

| Signal | Source |
|---|---|
| Unit price by half-hour | Energy supplier API |
| Live import power | Smart-meter data service (DCC) |
| Grid carbon intensity (forecast) | Public carbon-intensity APIs |
| Flexibility events | Supplier ⟨if enrolled⟩ |

| Load | Flexibility | Constraint |
|---|---|---|
| EV charger | High: hours | Target charge by departure |
| Dishwasher / washer-dryer | Medium: start delay | Finish by a set time; never interrupt a cycle |
| Workshop / 3D printers | Low: start delay | Operator consent |
| DHW reheat (later) | Medium | Cylinder minimum temperature |
