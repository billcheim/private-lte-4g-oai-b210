# Private LTE 4G Network with OAI and USRP B210

Documentation and deployment-oriented lab guide for building a private LTE 4G network using:

- OpenAirInterface (OAI)
- USRP B210
- Ubuntu Linux host
- Private SIM / USIM
- LTE user equipment (UE)

---

## Overview

This repository documents a practical lab workflow for building a private LTE network with OpenAirInterface and USRP B210.

It is intended for:

- telecom labs
- SDR experimentation
- LTE research
- private network demos
- educational deployments

---

## Features

- Real OAI installation workflow
- UHD / USRP detection steps
- EPC / Core startup sequence
- eNodeB startup example
- SIM provisioning notes
- UE attach flow
- Troubleshooting guide

---

## Architecture

```text
UE Device
   |
Private LTE Cell
   |
OAI eNodeB + USRP B210
   |
OAI EPC / Core
   |
IP Network
   |
External Services / Lab Network

## Quick Start

1. Prepare Ubuntu host

Install dependencies and tools.

2. Install UHD drivers

Detect the USRP B210 device.

3. Clone OpenAirInterface

Download the source code.

4. Build OAI

Compile eNodeB and core components.

5. Start the LTE network

Run EPC/Core and eNodeB.

See the docs folder for full commands and details.

---

## Documentation

- docs/hardware.md
- docs/install-oai.md
- docs/epc-setup.md
- docs/enodeb-setup.md
- docs/sim-provisioning.md
- docs/ue-attach.md
- docs/troubleshooting.md

---

## Scope

This repository is a lab and research guide.

Not intended for carrier-grade production use.

---

## Related Project

private-lte-voip-pbx

---

## License

MIT License
