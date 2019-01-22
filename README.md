# Seed Savior

A tool for recovering BIP39 seed phrases.
For more backgrounnd see [blog]
The tool is based on the bip39 project by Ian Coleman https://github.com/iancoleman/bip39

## Online Version

https://iancoleman.io/bip39/

## Standalone offline version

Download `mnemonic.html`

Open the file in a browser by double clicking it.

This can be compiled from source using the command `python compile.py`

## Usage

Enter your seed phrase into the 'BIP39 Phrase' field. If a word is missing or unknown, please type "?" instead and the tool will find all relevant options. If a word is wrong, the tool will try to suggest the closest option. 

The tool will suggest all relevant options for the missing word and the derived public addresses for Bitcoin anmd Ethereum. To find out if one of the suggested addresses is actually the right one, you can click on the suggested address  tocheck the address' transaction history on a block explorer.

## Demo

In this demo we enter "phrase brief ceiling dream rack install fault insane panic surround glory ? library brother hill sauce access child notice picnic dinner panda purity poem"

The tool suggests several options for the missing word and the relevant one will be "asset". We can verify that by clicking on the link of the dervied Ethereum address ("0x2dfF20b40504f99c6314ac30e8DF5c02dd8058e7" listed in the "BIP44 ETH Address" column) and checking the address has transaction history.

![Demo](/src/img/seed%20demo%20annotated.gif "Demo")


## Making changes

Please do not make modifications to `mnemonic.html`, since they will
be overwritten by `compile.py`.

Make changes in `src/*`.

Changes are applied during release using the command `python compile.py`, so
please do not commit changes to `mnemonic.html`



# License

This Seed Svior tool is released under the terms of the MIT license. See LICENSE for
more information or see https://opensource.org/licenses/MIT.
