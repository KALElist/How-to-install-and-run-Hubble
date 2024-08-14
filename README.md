
<table border=10 align=center>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/a52d56dc-49ef-431c-b2a1-c7f9e47e44cc" width=150></td>
  </tr>
</table>

This guide was made by user: KALElist

<h1 align=center> How-to-install-and-run-Hubble </h1>

## Install via Script
The install script is the simplest way to set up Hubble.

```bash
curl -sSL https://download.thehubble.xyz/bootstrap.sh | bash
```

## Upgrading Hubble
```bash
cd ~/hubble && ./hubble.sh upgrade
```

## Testnet
Set the following variables in your .env file in apps/hubble:
```bash
FC_NETWORK_ID=2
BOOTSTRAP_NODE=/dns/testnet1.farcaster.xyz/tcp/2282


If running from source code, add these arguments to the yarn start command
yarn start ... \
    -n 2 \
    -b /dns/testnet1.farcaster.xyz/tcp/2282
```
