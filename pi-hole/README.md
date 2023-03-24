# About

[Pi-hole](https://pi-hole.net/) is a self-hosted DNS server with built-in ad blocking. It can be used to block ads on all devices configured to use this as a DNS server.

This Docker Compose template is configured to run with a static IP address. It creates a network using the macvlan driver that binds it to a physical network interface (Ethernet or WiFi). The macvlan driver creates a virtual MAC address which is how it can claim a static IP on your router.

Tested with Docker version `20.10.21-ce`.

# Reset Password

After the Pi-hole container is up and running, run the following command to set/reset the password for the web UI:

`docker exec -it pihole sudo pihole -a -p`

# References

## About macvlan networks

* [Use macvlan networks (docs.docker.com)](https://docs.docker.com/network/macvlan/)
* [Using Docker macvlan networks (blog.oddbit.com)](https://blog.oddbit.com/post/2018-03-12-using-docker-macvlan-networks/)
