# Router Setup #

## Credentials ##
If you are a participant in this lab, do not log into the router. First, you will be ruining your own experience by messing with it. You will also be ruining the experience for other students. This information is provided here to allow the lab to be reproduced at a later time.

```
Username: root
Password: SuperSecurePassword!!1
```

## Image Creation ##
irst, install OpenWRT on your router. This is out of scope for this lab. I personally used the Netgear R6100. This configuration may not work with your router. Be careful. If you are not sure, the best thing is to manual set the settings to ensure nothing breaks.

Upload the [config file](./backup-OpenWrt-2019-01-30.tar.gz)

The wireless networks have the following configurations:

### WEP Network ###
```
SSID: `HackMePlease`
Key1: `MyPas`
```

I had to create the password using the following command. Note that the password has to be 5 characters long.
```
$ echo -n 'MyPas' | hexdump -e '5/1 "%02x" "\n"'
4d79506173
```

### WPA2 Network ###
```
SSID: `HackMePorFavor`
Password: `HelloThereHacker!`
```


