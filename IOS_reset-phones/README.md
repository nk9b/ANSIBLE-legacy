# ansible-reset-phones
            Ansible script to dynamically locate all access switch interfaces with attached IP Phones
This script will dynamically locate all interfaces on an access switch that are directly connected to an IP phone. The following actions are performed:

-   Locate all IP phone-connected interface(s).

-   Issue a shut/no shut on the interface(s).

Prerequisites:

-   Bash shell environment
