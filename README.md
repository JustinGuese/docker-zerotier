implementing a containerized version of zerotier based on bitnamis minideb image

https://www.zerotier.com

## usage

`docker run -e ZEROTIER_NETWORK=xxxxx guestros/zerotier`

## why?

i have some docker containers running on my server, and forward ports locally. unfortunately docker does not support UFW yet, meaning they are exposed to the world. I could play with iptables, but that is too much effort, and therefore i want to directly connect into the docker network using zerotier