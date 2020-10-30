# Troubleshoot IPsec tunnel

Commands to Verify if IPSec tunnel is up

```
tmsh show net ipsec ipsec-sa all-properties

tmsh show net ipsec ike-sa all-properties

tmsh show net ipsec-stat
```

In case the tunnel does not come up, check the IPsec log:

```
tail -f /var/log/ipsec.log
```

***

[back](BIG-IP_IKE_peer.md)

[IPSec config overview page](BIG_IP_IPsec_config.md)

[next](BIG-IP_virtual_server.md)