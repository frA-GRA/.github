# frA-GRA

Open Mission Systems (OMS) ecosystem implemented in Rust, plus tooling for integrating external systems with OMS-based architectures.

## What is OMS?

The Open Mission Systems (OMS) standard defines a Common Abstraction Layer (CAL) — a message-passing middleware that decouples mission-critical software components via a strongly-typed publish/subscribe bus. Components communicate through generated UCI schema messages over an Abstract Service Bus (ASB), with no direct dependency between publishers and subscribers.

## Repositories

| Repo | Description |
|------|-------------|
| [rcal](https://github.com/frA-GRA/rcal) | OMS Critical Abstraction Layer (CAL) implementation in Rust. Implements OMSC-SPC-001 CERT requirements. |
| [rcal-ardupilot](https://github.com/frA-GRA/rcal-ardupilot) | MAVLink-to-UCI gateway for ArduPilot SITL. Bridges ArduPilot autopilot telemetry into the OMS message bus. |
| [cosmos-oms](https://github.com/frA-GRA/cosmos-oms) | OpenC3/COSMOS plugin that translates OMS UCI messages to COSMOS telemetry and commands. |
| [frA-GRA](https://github.com/frA-GRA/frA-GRA) | Central hub: specifications, Docker examples, and git submodules for a complete system checkout. |

## Getting Started

Clone the hub repo with all submodules to get everything at once:

```bash
git clone --recurse-submodules https://github.com/frA-GRA/frA-GRA
```

See the [frA-GRA hub repo](https://github.com/frA-GRA/frA-GRA) for Docker Compose examples and full documentation.

## Specifications

OMS specifications and UCI schema summaries are archived in the [frA-GRA/specs](https://github.com/frA-GRA/frA-GRA/tree/main/specs) directory.

---

*Implementing [Open Mission Systems](https://www.openmissionsystems.org/) standards for the Rust ecosystem.*
