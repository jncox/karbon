.. _ILT

----------------
Pre-Requirements
----------------

For the workshop to work make sure the following requirements are met.

Nutanix Cluster
+++++++++++++++

Supported versions for the workhop:

- AOS 5.6.2.x
- AOS 5.8.2.x
- AOS 5.9.x
- AOS 5.10.x, preffered as that is being used in the workshop creation.

Supported Hypervisor:

- AHV, latest version preferred as that is being used in the workshop creation.


Extra settings needed:

- Virtual IP address and the ISCSI data service IP address configured.
- The cluster must be registered to Prism Central.
- Karbon requires a minimum 120 MB of memory and 700 MB of disk space in Prism Central.
- The cluster and Prism Central time zones must be synchronized.
- NTP and DNS must be configured.
- IPAM or DHCP network with access to the internet or a preconfigured unauthenticated proxy setup with access to the internet.


Cluster size:
-------------

- 1 node cluster minimum with a minimum of **128 GB** RAM per node

|

PRISM Central
+++++++++++++++

- PC 5.9 or later, preferred 5.10 as that is being used in the workshop creation.

|

Uploading images
++++++++++++++++

Two images to be installed in the cluster:

- CentOS version; look at :ref:`uploadimages` for installation process
- Ubuntu 16.0.4 LTS version; look at :ref:`uploadimages` for installation process

|

Karbon
++++++

- Tech Preview available in PRISM Central 5.10.x
- Enable Karbon process here :ref:`enable_karbon`
|

Attendee machine or VDI
+++++++++++++++++++++++

- Must have installed:
	
	1. kubectl; use :ref:`install_kubectl` to install kubectl.

- Nice to have installed:
	
	1. wget; use :ref:`install_wget` to install wget (for Windows **must** have, for Mac OS **nice** to have, for Linux it is built-in).

- Must have internet access.
