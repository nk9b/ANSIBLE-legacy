# ansible-locate-host
                    Ansible script to locate MAC/VLAN/IP/Interface mappings for edge hosts.

This script will display edge host connections attributes such as MAC/VLAN/IP/Interface mappings. The following steps are performed:

-   Log into the edge Cisco switch (L2/LAN switching only is supported).

-   Obtain dynamic node information from the CAM table.

-   Dynamically locate the default L3 interface for the VLAN.

-   Obtain MAC/ARP pairings from L3 interface/default gateway.

-   Merge and display the results of the CAM and ARP table queries.


Prerequisites:

-   Bash shell environment
