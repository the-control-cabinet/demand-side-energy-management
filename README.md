# Demand-Side Energy Management: Tariff-, Carbon- and Peak-Aware Load Control (Design Stage)

**BMS-style energy management for a home: shifting flexible loads (EV charging, appliances, workshop equipment) to cheap or low-carbon periods, limiting peak import demand, and responding to supplier demand-flexibility events, using live tariff, smart-meter and grid carbon-intensity data with comfort and safety constraints that always win.**

[![YouTube](https://img.shields.io/badge/YouTube-The%20Control%20Cabinet-red?logo=youtube)](https://www.youtube.com/channel/UC5Cupmz7vlfcodpCX7k8iuQ)
[![Portfolio](https://img.shields.io/badge/Portfolio-the--control--cabinet-24292f?logo=github)](https://github.com/the-control-cabinet/the-control-cabinet)
![Domain](https://img.shields.io/badge/BMS-demand%20response-blue)
![Status](https://img.shields.io/badge/Status-Design%20stage-yellow)

> **The short version:**
> - **Signals:** time-of-use tariff prices, live import (smart-meter data), grid carbon intensity, supplier flexibility events.
> - **Flexible loads:** the EV charger (largest), dishwasher/washer-dryer (appliance hub), workshop and 3D printers, and later boiler/DHW timing via the OpenTherm stage.
> - **Strategies:** cheapest/cleanest-window scheduling, **peak-demand limiting** (shed or defer loads above an import threshold), event response.
> - **Constraints:** a car charged by departure time, comfort bands for heating, no interruption of running appliance cycles.

**Portfolio position:** Management level · energy management. Builds on: [energy dashboard](https://github.com/the-control-cabinet/home-energy-dashboard) (metering, tariffs, M&V). Coordinates with: [OpenTherm control](https://github.com/the-control-cabinet/opentherm-boiler-control-esphome) · [supervisory layer](https://github.com/the-control-cabinet/ha-node-red-supervisory-layer)

---

## Documents

| Doc | Contents |
|---|---|
| [01 Signals and loads](docs/01-signals-and-loads.md) | What's measured, what can move |
| [02 Strategies](docs/02-strategies.md) | Scheduling, peak limiting, event response |
| [03 Measurement](docs/03-measurement.md) | Savings and verification |

## Roadmap
- [ ] Signals into HA (prices, import, carbon)
- [ ] EV cheapest-window charging
- [ ] Peak limiter in shadow mode
- [ ] Appliance start-delay scheduling
- [ ] Savings report

## Skills demonstrated (as built)
| Skill | Evidence |
|---|---|
| Energy management | Tariff and carbon-aware scheduling |
| Demand response | Peak limiting and event response |
| Constraint handling | Comfort and safety constraints always win |
| M&V | Cost, carbon and peak savings measured |

📺 [The Control Cabinet on YouTube](https://www.youtube.com/channel/UC5Cupmz7vlfcodpCX7k8iuQ)

*Built and documented by James · part of [The Control Cabinet BMS portfolio](https://github.com/the-control-cabinet/the-control-cabinet). MIT Licence.*
