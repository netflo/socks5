# socks5


#client proxy command:
ssh -N -D 0.0.0.0:1080 localuser@localhost   |> could become auto ssh connect

#test with:
ncat --proxy proxy_ip:1080  --proxy-type socks5  client_network_ip  client_port

#client:
ncat -l 888  (listening port = 888)

##########################################


systemd-resolved looks after local application DNS responses. 

Disable systemd-resolved and reboot. nameserver 127.0.0.53 is not written to /etc/resolv.conf.

sudo systemctl disable systemd-resolved
sudo reboot



###########################
