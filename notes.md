## Inetd way

```sh
sudo apt install inetutils-telnetd inetutils-inietd
sudo update inetd --enable telnet
sudo /etc/init.d/inetutils-inetd restart
```

## Xinetd way

```sh
sudo apt-get install xinetd telnetd
# For editing config files view
sudo /etc/init.d/xinetd restart
# check status
```

## Solve permission issues for wireshark
Logout and login as necessary
```sh
$ sudo adduser $USER wireshark
$ sudo chown root /usr/bin/dumpcap
$ sudo chmod u+s /usr/bin/dumpcap
```
