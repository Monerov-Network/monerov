# Monerov

Monerov is based on [Monero](README_original.md)  


## Resources

- Webpage: [monerov.network](http://monerov.network)
- Explorer Mainnet: [explorer.monerov.online](https://explorer.monerov.online/)
- Explorer Testnet: [explorer.test.monerov.online](https://explorer.test.monerov.online/)
- Official Pool Mainnet: [pool.monerov.online](https://pool.monerov.online/)
- Official Pool Testnet: [pool.test.monerov.online](https://pool.test.monerov.online/)
- GUI Wallet Downloads: [github.com/xmvdev/monerov-gui/releases](https://github.com/xmvdev/monerov-gui/releases)

## Social/Contact

- Telegram: 
- Discord: 
- Twitter: [twitter.com/monerovofficial](https://twitter.com/monerovofficial)
- Email: xmvdev@gmail.com

## Specifications & Emission

- Coin ticker: XMV
- Total supply: 27,000,000 coins before tail emission
- Tail emission: ~158,000 coins each year (starting at year 8)
- Decimal places: 11
- PoW hash algorithm: RandomV
- Block time: 60 seconds
- Difficulty Adjustment Algorithm: Monero DAA
- Premine: 5,300,000 (to be distributed to monerov v1 holders)
- Devmine: 2,700,000 (locked for 2 years)
- Mainnet default P2P port: 19280
- Mainnet default RPC port: 19281

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

