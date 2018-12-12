# socks5


#client proxy command:
ssh -N -D 0.0.0.0:1080 localuser@localhost   |> could become auto ssh connect

#test with:
ncat --proxy proxy_ip:1080  --proxy-type socks5  client_network_ip  client_port

#client:
ncat -l 888  (listening port = 888)
