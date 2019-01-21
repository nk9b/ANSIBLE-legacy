# ansible-napalm-baseline
                  NAPALM Ansible module for performing NAPALM-related provisioning/configuration tasks

This script utilizes the napalm-ansible module. The following steps are performed:

-   NAPALM is set to REPLACE (not MERGE) the existing system configuration, then commit the change.

-   Cisco IOS' file archive feature is utilized; the script generates a candidate configuration, SCPs the configuration template to the device, then issues a "configuration replace" function within the archive.

-   If an error is thrown by IOS, the previous configuration is automatically rolled-back.

Prerequisites:

-   napalm-ansible module

-   Cisco IOS "archive" feature set

-   A bootstrap network connectivity configuration for the device
