# EPC / Core Setup

## Components

Typical LTE EPC includes:

- MME
- HSS
- SPGW

## Responsibilities

- UE authentication
- IP address assignment
- mobility management
- packet routing

## Example Flow

1. Start database services if required
2. Start HSS
3. Start MME
4. Start SPGW
5. Verify interfaces are up

## Validation

- UE can attach
- UE receives IP address
- UE can route traffic

## Notes

Configuration depends on OAI release and selected deployment model.
