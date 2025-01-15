# Raspberry Pico Starter Code

## Environment setup
1. cd /opt
2. git pull https://github.com/raspberrypi/pico-sdk.git --branch master
3. cd pico-sdk/
4. git submodule update --init
5. export PICO_SDK_PATH=/opt/pico-sdk

## Update SDK
1. cd /opt/pico-sdk
2. git pull
3. git submodule update

## To build
1. Replace <BOARD_NAME_HERE> in CMakeLists.txt with name of development board
2. Replace <PROJECT_NAME_HERE> in CMakeLists.txt with project name
3. bash scripts/build.sh

## To clean
1. Run 'bash scripts/clean.sh' to delete all build files from the build/ directory

## To load on Raspberry PICO
1. Hold BOOTSEL button and plug PICO into USB
2. Copy build/<PROJECT_NAME_HERE>.uf2 to RPI-RP2 Volume
