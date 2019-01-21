# ansible-update-ios
                    Ansible script to update Catalyst IOS device images

This script will intelligently update the image of the defined Catalyst IOS device platform. The following summarized update procedure is performed:

-   Task includes are used instead of roles; each include calls a device-specific task list.

-   Check the version of currently running image; delete directories and all other binaries except for currently running image.

-   Transfer image, perform MD5 checksum, update boot variable, and schedule device reload.

Prerequisites:

-   Bash shell environment

