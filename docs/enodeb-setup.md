# eNodeB Setup (USRP B210)

## Goal

Configure and start the LTE eNodeB using OpenAirInterface and USRP B210.

## Verify SDR Detection

uhd_find_devices

## Example Config Path

~/openairinterface5g/targets/PROJECTS/GENERIC-LTE-EPC/CONF/

## Typical Parameters to Review

- downlink_frequency
- uplink_frequency_offset
- eutra_band
- N_RB_DL
- tracking_area_code
- mobile_country_code
- mobile_network_code
- tx_gain
- rx_gain

## Start eNodeB Example

cd ~/openairinterface5g/cmake_targets/ran_build/build

sudo ./lte-softmodem \
-O ~/openairinterface5g/targets/PROJECTS/GENERIC-LTE-EPC/CONF/enb.band7.tm1.25PRB.usrpb210.conf

## Validation

- USRP initializes
- RF sync successful
- Cell starts broadcasting
- UE can detect LTE cell

## Troubleshooting

If startup fails:

- check USB 3.0 connection
- check UHD version
- verify config file path
- lower gain settings
- review console logs
