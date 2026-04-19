# eNodeB Setup

## Purpose

The eNodeB provides LTE radio access between UE devices and the EPC/Core.

## Hardware

- USRP B210
- USB 3.0 host system
- LTE antennas

## Typical Configuration Items

- LTE band
- EARFCN / frequency
- bandwidth
- PLMN
- TAC
- transmit gain
- sample rate

## Startup Flow

1. Connect USRP B210
2. Confirm host detects SDR
3. Load eNodeB configuration
4. Start eNodeB service
5. Verify synchronization

## Validation

- UE sees LTE cell
- UE attempts attach
- Core receives signaling
