# ansible-check-bpduguard-status
                    Ansible script to check Catalyst IOS interfaces in BPDUGuard error-disable state

This script will check for Catalyst IOS edge interfaces that are in an error-disable state due to active BPDUGuard action. The following checks/steps are performed:

-   Discover all interfaces that are error-disabled caused by BPDUGuard.

-   Administratively shut these interfaces.

-   Update the interface descriptions as "*** LOOPED INTERFACE ***" for manual review by network operations staff.

-   Parse the device syslog:

    -   Sort entries by the current day.
    
    -   Count the number of interface flaps/error-recovery attempts by the device.
    
-   Email results to network operations staff.

Prerequisites:

-   Error-recovery within Catalyst IOS

-   SMTP/MTA for email functionality

-   Bash shell environment
