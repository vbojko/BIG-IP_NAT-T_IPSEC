# Troubleshooting Tips

If the tunnel does not successfully establish, here are a few things to check.<br>
Please note: This is not an exhaustive list.

## Virtual Server(s)
The more specific the Virtual Server source and destination addresses are, the greater chance of the tunnel not establishing, if the addresses are incorrect.  These addresses should be the private networks or hosts that the networks or hosts on the other side of the tunnel need to communicate with.  In this context, "private" means not accessible from the public Internet.  They may or may not use RFC1918 address space.<br>

Consider temporarily testing with a wildcard (0.0.0.0) virtual server to eliminate this possibility.

## Tunnels Object
The BIG-IP Tunnels object is not used with IPSec use cases.<br>

Consider deleting any tunnel objects that are unused or inactive.

## Reboot
Changing IPSec configuration objects may require rebooting BIG-IP in order for those changes to take effect.<br>

Please note: BIG-IP may not provide any indication of this requirement.

***

[back to README](../README.md)

[next](BIG-IP_IPsec_policy.md)
