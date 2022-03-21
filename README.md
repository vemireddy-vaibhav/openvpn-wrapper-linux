# openvpn-wrapper-linux

## Pre-configuration tasks
```bash
$ chmod +x vpncli
$ sudo mv vpncli /usr/local/bin
$ vpncli
$ cd $HOME/.vpncli/profiles
$ mkdir {{ profile }}
```


Inside the profile directory, we should have two files.
  - `.ovpn` config file
  - `{{ profile }}.auth` (Must have username, password for ovpn authentication)

`$ chmod 600 $HOME/.vpncli/profiles/{{ profile }}/{{ profile }}.auth`

## Usage
```bash
$ vpncli -h
Usage:  $(basename "$0") [-h] [-d] [-s] [-l] [-p <PROFILE_NAME>]

Where:  -h  show this help text
        -d  disconnect from VPN
        -s  show connected profile
        -l  list profiles
        -p  connect using the specified profile

```
 
