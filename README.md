# wireguard-multihop
This repository contains my wireguard config for setting up a multihop VPN.  
I use an OCI-VPS (Ubuntu) as first hop.  
From there the connection is redirected to my OPNsense and I can use my selfhosted services.


Client: The device you want to connect/to use.

First-Hop: OCI = Oracle Cloud Infrastructure (I use the free tier).

Second-Hop: OPNsense


## Attention: 

This is specifically designed for Ubuntu

You have to flush your iptables after every restart of your ubuntu instance.
You can use a script, that flushes the iptables and starts wireguard.

If you dont have a public IP for your OPNsense, you can use a DynDNS-Serice. 


You have to configure your OPNsense to activate your wg-interface in the right way. (Road-Warrior-Setup (see offical OPNsense Docs) 
