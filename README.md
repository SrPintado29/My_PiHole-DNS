# My_PiHole-DNS

  My Pi-Hole system on Raspberry pi 3+. 
  Commands and system configuration. 
  Hardening and securization of Raspbian, SSH and Fw. 
  Compilation of my Blacklists and regular expressions (Reggex).

#> Descripcion of my Pi Hole system: 

  Pi Hole is used to prevent Internet tracking and to block advertisements. This system works at the network level under a Linux distribution and functions as a DNS and DHCP server opcional. 

  In my particular case, I have configured Pi-Hole as a network proxy connected to my FTTH router. The network traffic from my hosts that I want to pass through Pi Hole I route it through the Pi Hole IP address set as DNS. 

  I do this type of proxy routing because my personal router does not allow to change in its options the primary DNS nor the secondary DNS and definitely, I have to change it in each of my devices. This allows me to have more flexibility in selecting which host I want to route to my proxy network.

Otherwise, you can cofigure your Pi Hole as a recursive dns. This type of dns can be reached through the Unbound service intalled on your Raspbian system. This service allows you to put your Pi Hole as a locally cached dns on your private network, improving your privacy even more but reducing your connection speed.
