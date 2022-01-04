# pywallet (CLI)
[![PyPI version](https://badge.fury.io/py/bip-utils.svg)](https://badge.fury.io/py/bip-utils)
[![Build Status](https://travis-ci.com/ebellocchia/bip_utils.svg?branch=master)](https://travis-ci.com/ebellocchia/bip_utils)
[![codecov](https://codecov.io/gh/ebellocchia/bip_utils/branch/master/graph/badge.svg)](https://codecov.io/gh/ebellocchia/bip_utils)
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/9a0c9c6a3d6444fab91f58fe8ec9e35c)](https://www.codacy.com/gh/ebellocchia/bip_utils/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ebellocchia/bip_utils&amp;utm_campaign=Badge_Grade)
[![CodeFactor](https://www.codefactor.io/repository/github/ebellocchia/bip_utils/badge)](https://www.codefactor.io/repository/github/ebellocchia/bip_utils)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://raw.githubusercontent.com/ebellocchia/bip_utils/master/LICENSE)

Wallet importer/exporter for Bitcoin (BTC), BTG, BCH, LTC, DASH, USDT, QTUM and DOGE 

# Linux Usage
    sudo ./pywallet-cli

# Windows Usage
    Execute pywallet.exe in CLI (cmd.exe)

# Arguments                      
      --version             show program's version number and exit
      -h, --help            show this help message and exit
      --dump_bip32=DUMP_BIP32
                            dump the keys from a xpriv and a path, usage:
                            --dump_bip32 xprv9s21ZrQH143K m/0H/1-2/2H/2-4
      --bip32_format=BIP32_FORMAT
                            format of dumped bip32 keys
      --passphrase=PASSPHRASE
                            passphrase for the encrypted wallet
      --find_address=FIND_ADDRESS
                            find info about an address
      -d, --dumpwallet      dump wallet in json format
      --dumpformat=DUMPFORMAT
                            choose what to extract in a wallet dump
      --dumpwithbalance     includes balance of each address in the json dump,
                            takes about 2 minutes per 100 addresses
      --importprivkey=KEY   import private key from vanitygen
      --importhex           DEPRECATED, useless
      --datadir=DATADIR     REMOVED OPTION: put full path in the --wallet option
      -w WALLETFILE, --wallet=WALLETFILE
                            wallet filename (defaults to wallet.dat)
      --label=LABEL         label shown in the adress book (defaults to '')
      --testnet             use testnet subdirectory and address type
      --namecoin            use namecoin address type
      --eth                 use ethereum address type
      --otherversion=OTHERVERSION
                            use other network address type, either P2PKH prefix
                            only (e.g. 111) or full network info as
                            'name,p2pkh,p2sh,wif,segwithrp' (e.g. btc,0,0,0x80,bc)
      --info                display pubkey, privkey (both depending on the
                            network) and hexkey
      --reserve             import as a reserve key, i.e. it won't show in the
                            adress book
      --multidelete=MULTIDELETE
                            deletes data in your wallet, according to the file
                            provided
      --balance=KEY_BALANCE
                            prints balance of KEY_BALANCE
      --recover             recover your deleted keys, use with recov_size and
                            recov_device
      --recov_device=RECOV_DEVICE
                            device to read (e.g. /dev/sda1 or E: or a file)
      --recov_size=RECOV_SIZE
                            number of bytes to read (e.g. 20Mo or 50Gio)
      --recov_outputdir=RECOV_OUTPUTDIR
                            output directory where the recovered wallet will be
                            put
      --clone_watchonly_from=CLONE_WATCHONLY_FROM
                            path of the original wallet
      --clone_watchonly_to=CLONE_WATCHONLY_TO
                            path of the resulting watch-only wallet
      --dont_check_walletversion
                            don't check if wallet version > 81000 before running
                            (WARNING: this may break your wallet, be sure you know
                            what you do)
      --random_key          print info of a randomly generated private key
      --whitepaper          write the Bitcoin whitepaper using bitcoin-cli or
                            blockchain.info
      --minimal_encrypted_copy
                            write a copy of an encrypted wallet with only an empty
                            address, *should* be safe to share when needing help
                            bruteforcing the password
      --tests               run tests
      

## Donation ##
If you find this program helpful, please consider a donation:

BTC: bc1qqtspvvyl5nv2dwffd0zwppledlmct7sydpd9l5

**Thank You!**

