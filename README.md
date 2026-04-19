# Private LTE 4G Network with OAI and USRP B210

Documentation and demo project for building a private LTE 4G network using:

- OpenAirInterface (OAI)
- USRP B210
- Linux host system
- Private SIM / USIM
- LTE user equipment (UE)

---

## Overview

This repository documents a lab-style deployment of a private LTE network.

It focuses on education, experimentation, and research-oriented setups.

---

## Features

- Example OAI installation workflow
- EPC / Core network notes
- eNodeB setup guidance
- SIM provisioning notes
- UE attach workflow
- Troubleshooting guides
- Integration path for VoIP / PBX services

---

## Architecture

UE Device  
↓  
Private LTE eNodeB  
↓  
OAI EPC / Core  
↓  
IP Network  
↓  
External Services (PBX / Internet / Lab)

---

## Included Documentation

- hardware.md
- install-oai.md
- epc-setup.md
- enodeb-setup.md
- sim-provisioning.md
- ue-attach.md
- troubleshooting.md

---

## Scope

This repository is intended for:

- telecom labs
- LTE research
- SDR experimentation
- private network demonstrations

Not intended as a carrier-grade production deployment.

---

## License

MIT License

