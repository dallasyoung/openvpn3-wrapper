# openvpn3-wrapper

This simple Bash script wraps the most common VPN control operations you will
use with the
[OpenVPN 3 Client for Linux](https://openvpn.net/cloud-docs/owner/connectors/connector-user-guides/openvpn-3-client-for-linux.html).
The program is fairly well documented, but the CLI is a bit clunky and kind of
a PITA to actually use, so this script is just meant to be a bit more
consistent & to cut down on typing when you actually need to use your VPN

Note that this script does not manage any aspects of setting up an OpenVPN
server, nor does it import any `.ovpn` configs. You must do this all yourself
first

## Prerequisites

  - Bash
  - The [OpenVPN 3 Client for Linux](https://openvpn.net/cloud-docs/owner/connectors/connector-user-guides/openvpn-3-client-for-linux.html) installed

## Setup

```
git clone https://github.com/dallasyoung/openvpn3-wrapper
cd openvpn3-wrapper
chmod +x ./vpn
```

## Usage 

To connect your VPN:

```
./vpn connect <profile name>
```

To disconnect your VPN:

```
./vpn disconnect <profile name>
```

To show your current connections:

```
./vpn status
```
