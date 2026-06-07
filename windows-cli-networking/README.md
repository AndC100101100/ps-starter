# Overview

## ipconfig
checking the network settings for the local machine. By opening up Command Prompt and typing ipconfig you can access the current settings. 

```shell
ipconfig
```

## netsh
used to start Network shell which can be used to manage the network settings of the local and or a remote computer

`netsh interface ip set address <connection name> static <IP> <subnet> <gateway>`

```shell
netsh interface ip set address "Ethernet0" static 172.16.16.150 255.255.255.0 172.16.16.1
```

## net 
We can mount shared folders by using the 'net' command. This command is used to manage almost all aspects of a network and its settings including shares, print jobs and users. `net /?` for all commands

to mount a network drive you need:
```shell
net use x: \\DESKTOP-3VSCDO9\Share
```

to remove a mounted drive 
```shell
net use x: \\DESKTOP-3VSCDO9\Share
```
