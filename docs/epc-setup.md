# EPC / Core Setup (Real Guide)

## Goal

Start the LTE core network required for UE attachment.

## Typical Components

- HSS
- MME
- SPGW

## Example Start Order

cd ~/openairinterface5g/cmake_targets/ran_build/build

## Start HSS

sudo ./oai_hss

## Start MME

sudo ./oai_mme

## Start SPGW

sudo ./oai_spgw

## Validation

Check:

- services remain running
- interfaces created
- no critical errors in logs

## Then Start eNodeB

After EPC is running, start the eNodeB.

## Then Attach UE

Insert provisioned SIM and test registration.

## Notes

Binary names can vary by OAI release.
Use the build output of your selected branch.
