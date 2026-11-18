# denarius

denarius is a cryptocurrency node and wallet for transferring D over a peer-to-peer network. It combines Tribus Proof of Work with Proof of Stake and supports optional privacy tools, atomic swaps, and IPFS integration. This standalone project is based on metaspartan/denarius.

## Features

- Mine blocks with the Tribus Proof-of-Work algorithm or participate through Proof of Stake.
- Run Fortuna Stakes, the hybrid masternode system, with 5,000 D collateral.
- Exchange assets through UTXO-based atomic swaps using BIP65 CLTV.
- Enable the native Tor onion node with `nativetor=1`.
- Upload files to IPFS through the Jupiter UI and RPC integration.
- Register decentralized domain names through the Denarius Name-Value System (NVS).

## Installation

The inherited installation instructions use Snap on Linux. These commands install the existing Denarius package; they do not build or install this standalone repository.

On Debian or Ubuntu:

```sh
sudo apt install snapd
sudo snap install denarius
```

The package provides the graphical wallet as `denarius` and the daemon as `denarius.daemon`.

For a source build of this standalone project, use its checked-in build instructions. The donor information does not provide a verified compiler, dependency list, or build command, so no source-build recipe is included here.

## Usage

Start the graphical wallet from the Snap installation:

```sh
denarius
```

Alternatively, run the node daemon:

```sh
denarius.daemon
```

To enable native Tor support, add this setting to `denarius.conf` before starting the node:

```ini
nativetor=1
```

Tor support is optional and does not by itself guarantee anonymity. Back up your wallet before upgrading or changing your installation.

## License

MIT. This project is based on [metaspartan/denarius](https://github.com/metaspartan/denarius). Retain the original copyright and MIT permission notices when redistributing the code or substantial portions of it.
