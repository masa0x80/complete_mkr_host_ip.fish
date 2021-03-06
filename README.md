# complete_mkr_host_ip.fish

[![MIT LICENSE](http://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](LICENSE)

## Overview

Fish plugin for completing IP address of host registered to [mackerel].

## Installation

With [fresco]
```
fresco masa0x80/complete_mkr_host_ip.fish
```

With [fisherman]
```
fisher masa0x80/complete_mkr_host_ip.fish
```

## Dependencies

- [mkr]
- [jq]
- [fzf]

## Usage

To insert IP address to command line, type ctrl-o ctrl-o (`\co\co`).

## Setup

### `MACKEREL_APIKEY`

**required**

To use mkr, you should assign the API key to the environment variable.

### `MACKEREL_APIKEY_NAME`

It is a suffix of cache file. The cache file of `complete_mkr_host_ip.fish` is separated by using `MACKEREL_APIKEY_NAME`.
If you use *mackerel organizations*, I think it is useful to specify `MACKEREL_APIKEY_NAME`.

### `MKR_HOSTS_TSV_GIP`

It is defaulted to 'false'. If you want to complete global IP address, you should set it 'true'.

### `COMPLETE_MKR_HOST_IP_KEYBIND`

`COMPLETE_MKR_HOST_IP_KEYBIND` is the key binding to start the input completion for host's IP address.
It is defaulted to `\co\co` (ctrl-o ctrl-o).

## Bibliography

- [Mackerel + peco + zsh でコマンドラインにホスト名を補完する](http://motemen.hatenablog.com/entry/2015/07/mackerel-mkr-peco-zsh)

[mackerel]: https://mackerel.io/mackerel
[mkr]: https://github.com/mackerelio/mkr
[jq]: https://stedolan.github.io/jq/
[fzf]: https://github.com/junegunn/fzf
[fresco]: https://github.com/masa0x80/fresco
[fisherman]: https://github.com/fisherman/fisherman
