# Monerov

Monerov is based on [Monero](README_original.md)  


## Resources

- Webpage: [monerov.online](http://monerov.online)
- Explorer: [explorer.monerov.online](https://explorer.monerov.online/)
- GitHub: [github.com/xmvdev](https://github.com/xmrdev)

## Social/Contact

- Telegram: 
- Discord: 
- Twitter: [twitter.com/monerovofficial](https://twitter.com/monerovofficial)
- Email: xmvdev@gmail.com

## Specifications & Emission

- Coin ticker: XMV
- Total supply: 18,400,000 coins before tail emission
- Tail emission: ~158,000 coins each year (starting at year 8)
- Decimal places: 12
- PoW hash algorithm: CryptoNightV7
- Block time: 60 seconds
- Difficulty Adjustment Algorithm: Monero DAA
- Premine: 5,000,000 (to be distributed to monerov v1 holders)
- Mainnet default P2P port: 19250
- Mainnet default RPC port: 19251

## Build on linux

install deps:

`sudo apt-get install build-essential cmake pkg-config libboost-all-dev libssl-dev libzmq3-dev libunbound-dev libsodium-dev libreadline6-dev libpgm-dev libnorm-dev`

clone repo:

`git clone --recursive https://github.com/xmvdev/monerov`

build daemon and wallet:

`cd monerov && mkdir build && cd build && cmake .. && make daemon simplewallet`

or build everything:

`cd monerov && mkdir build && cd build && cmake .. && make`

## Build on Windows (using MinGW)

install deps:

`pacman -S mingw-w64-x86_64-toolchain make mingw-w64-x86_64-cmake mingw-w64-x86_64-boost mingw-w64-x86_64-openssl mingw-w64-x86_64-zeromq mingw-w64-x86_64-libsodium mingw-w64-x86_64-hidapi`

clone repo:

`git clone --recursive https://github.com/xmvdev/monerov`

build daemon and wallet:

`cd monerov && make release-static-win64`

