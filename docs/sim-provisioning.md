# SIM Provisioning (Practical Guide)

## Goal

Provision a private SIM / USIM so the UE can authenticate to the LTE core.

## Typical Subscriber Parameters

- IMSI
- Ki
- OPC or OP
- APN
- MSISDN (optional)

## Practical Workflow

1. Create subscriber record in the HSS database
2. Program the SIM card with matching credentials
3. Insert the SIM into the UE
4. Power on the UE
5. Attempt LTE attach

## Example Validation

Confirm that:

- IMSI matches the HSS entry
- authentication succeeds
- UE receives IP address
- data session becomes active

## Notes

Exact tools depend on the SIM programming workflow used in your lab.

Use lab-only credentials and handle subscriber secrets carefully.
