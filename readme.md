# UPDATE #

**To keep up with Coinomi great work, I'll have to redesign my solution to separate file to fully isolate changes**

**Technically creating BIP39 recovery phrase from custom phrase (brain wallet) can be totally separate file and potentially just merged during compilation. Worst case scenario two file solution, and copy/paste words from one to the other**

# BIP39 Tool with Personal Passphrase

A tool for converting BIP39 mnemonic phrases to addresses and private keys.

## Online Version

[https://greenhex.net/bip39-personal-standalone.html](https://greenhex.net/bip39-personal-standalone.html "https://greenhex.net/bip39-personal-standalone.html")

## Standalone offline version

Download `bip39-personal-standalone.html`

Open the file in a browser by double clicking it.

This can be compiled from source using the command `python compile.py`

## Usage

Enter your personal phrase into the 'Your custom Passphrase' field. Your Bip39 will be re-generated from this.

Or

Enter your BIP39 phrase into the 'BIP39 Phrase' field, or press
'Generate Random Phrase'

If required, set the derivation path, although the defaults are quite usable, just use 'Coin' dropdown to select a coin for which the addresses to be generated. 

See the table for a list of addresses generated from the phrase.

Toggle columns to blank to easily copy/paste a single column of data, eg to
import private keys into a wallet or supply someone with a list of addresses.

Click the addresses or keys to toggle view of a QR code of same address.

Click the Show QR buttons by the root key and extended public and private keys to show a qr code suitable 
for importing into a wallet on a mobile device.

The BIP32 keys can be used at [bip32.org](https://bip32.org) if desired.

## Making changes

Please do not make modifications to `bip39-personal-standalone.html`, since they will
be overwritten by `compile.py`.

Make changes in `src/*` and apply them using the command `python compile.py`
