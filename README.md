# QuickTinc

Here's a script to quickly setup a VPN using tinc. This makes use of docker, image `jenserat/tinc`. You basically only have to install Docker to get started.

## Getting Started

You can find a [tutorial to setup a mini VPN with quicktinc here](https://fovea.cc/blog/index.php/docker-on-tinc-in-docker/).

## Usage

```
Usage:
./quicktinc [OPTIONS]

Options:
   --net=NET_NAME           Network name (required)
   --node=NODE_NAME         Node name (required)
   --public-ip=PUBLIC_IP    Node's public IP (required)
   --private-ip=PRIVATE_IP  Node's private IP (required)
   --connect-to=HOST        Name of another node (optional, repeatable)
   --interface=tun0         Network interface to create (optional, default=tun0)
   --config=/srv/tinc       Where to save tinc networks (optional, default=/srv/tinc)
   --up                     Also start the daemon
```

## License

(c)2015, Jean-Christophe Hoelt

Published under GPL v2.
