# SIM Provisioning

## Purpose

Private LTE deployments require SIM / USIM identities recognized by the core network.

## Typical Parameters

- IMSI
- Ki
- OPC or OP
- MSISDN (optional)
- APN
- subscriber profile

## Workflow

1. Create subscriber entry in HSS database
2. Program SIM card with matching identity
3. Insert SIM into UE device
4. Power on UE and attempt attach

## Validation

- UE authenticates successfully
- UE receives IP address
- Data session is active

## Notes

Use lab-only subscriber data and secure handling of credentials.
