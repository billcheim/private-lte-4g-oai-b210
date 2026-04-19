# Install OpenAirInterface (Real Build Guide)

## Tested Host OS

- Ubuntu 22.04 LTS recommended

## Update System

sudo apt update
sudo apt upgrade -y

## Install Basic Dependencies

sudo apt install -y git curl wget vim cmake build-essential pkg-config \
python3 python3-pip python3-dev \
libboost-all-dev libusb-1.0-0-dev \
libfftw3-dev libsctp-dev lksctp-tools \
iproute2 net-tools pciutils

## Install UHD (USRP Drivers)

sudo apt install -y uhd-host libuhd-dev

## Verify USRP Detection

uhd_find_devices

Expected output should list USRP B210.

## Update FPGA Images

sudo uhd_images_downloader

## Clone OpenAirInterface

cd ~
git clone https://gitlab.eurecom.fr/oai/openairinterface5g.git
cd openairinterface5g

## Checkout Stable Branch

git branch -a

Select a stable release branch if required.

## Install OAI Dependencies

cd cmake_targets
./build_oai -I

## Build eNodeB

./build_oai -w USRP --eNB

## Build EPC/Core (legacy workflow if required)

./build_oai --core

## Notes

Build options may vary by OAI release.
Always verify current official documentation.
