**Introduction**

This solution uses an ARM template to launch a three NIC deployment of a cloud-focused BIG-IP VE in Microsoft Azure. This template can optionally also add additional NIC(s) to the BIG-IP to be used as needed. Traffic flows from the BIG-IP VE to the application servers. This is the standard on-premise-like cloud design where the BIG-IP VE instance is running with a management, front-end application traffic (Virtual Server) and back-end application interface.

The BIG-IP VE has the Local Traffic Manager (LTM) module enabled to provide advanced traffic management functionality. This means you can also configure the BIG-IP VE to enable F5's L4/L7 security features, access control, and intelligent traffic management.

For information on getting started using F5's ARM templates on GitHub, see Microsoft Azure: Solutions 101.

Networking Stack Type: This template deploys into an existing networking stack; so the networking infrastructure MUST be available prior to deploying. See the Template Parameters Section for required networking objects.
