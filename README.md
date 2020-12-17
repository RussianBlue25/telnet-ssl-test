# telnet-ssl-test

A test repository for telnet-ssl.
This needs docker and docker-compose.

# How It Works
```
cd telnet-ssl # If you test normal telnet, change telnet-ssl to telnet-normal.
docker-compose build
docker-compose up -d
```

## client
```
docker exec -it telnet-ssl-client bash # If you test normal telnet, change telnet-ssl to telnet-normal.

$ telnet telnet-ssl-server 23 # If you test normal telnet, change telnet-ssl to telnet-normal.
```
Both telnet-ssl and telnet-normal are the same command.
User for telnet is "docker", its password is "docker", too.

A pcap file is created under the pcap directory.
(Default name is telnet-normal.pcap or telnet-ssl.pcap)
