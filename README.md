# openvpn-wrapper-linux

```bash
$ chmod +x vpncli
$ sudo mv vpncli /usr/local/bin
$ vpncli -h
$ cd $HOME/.vpncli/profiles
$ mkdir {{ profile }}
```


Inside the profile directory, we should have two files.
  - `.ovpn` config file
  - `{{ profile }}.auth` (Must have username, password for ovpn authentication)

`$ chmod 600 $HOME/.vpncli/profiles/{{ profile }}/{{ profile }}.auth`
 
