.. title:: Nutanix Karbon Workshop

.. toctree::
  :maxdepth: 2
  :caption: Karbon 1.0
  :name: _karbon_1_0
  :hidden:

  karbon/karbon

.. _getting_started:

---------------
Getting Started
---------------

Welcome to the Nutanix Karbon Labs! This workbook accompanies an instructor-led session that introduces Nutanix Karbon and many common management tasks.
Each section has a lesson and an exercise to give you hands-on practice.
The instructor explains the exercises and answers any additional questions that you may have.

What's New
++++++++++

- Workshop updated for the following software versions:
    - AOS|PC 5.10

Initial Setup
+++++++++++++

- Take note of the *Passwords* being used.
- Log into your virtual desktops (connection info below)

Environment Details
+++++++++++++++++++

Nutanix Bootcamps are intended to be run in the Nutanix Hosted POC environment. Your cluster will be provisioned with all necessary images, networks, and VMs required to complete the exercises.

Networking
..........

Hosted POC clusters follow a standard naming convention:

- **Cluster Name** - POC\ *XYZ*
- **Subnet** - 10.**21**.\ *XYZ*\ .0
- **Cluster IP** - 10.**21**.\ *XYZ*\ .37

If provisioned from the marketing pool:

- **Cluster Name** - MKT\ *XYZ*
- **Subnet** - 10.**20**.\ *XYZ*\ .0
- **Cluster IP** - 10.**20**.\ *XYZ*\ .37

For example:

- **Cluster Name** - POC055
- **Subnet** - 10.21.55.0
- **Cluster IP** - 10.21.55.37

Throughout the Bootcamp there are multiple instances where you will need to substitute *XYZ* with the correct octet for your subnet, for example:

.. list-table::
  :widths: 25 75
  :header-rows: 1

  * - IP Address
    - Description
  * - 10.21.\ *XYZ*\ .37
    - Nutanix Cluster Virtual IP
  * - 10.21.\ *XYZ*\ .39
    - **PC** VM IP, Prism Central
  * - 10.21.\ *XYZ*\ .40
    - **DC** VM IP, NTNXLAB.local Domain Controller

Each cluster is configured with 2 VLANs which can be used for VMs:

.. list-table::
  :widths: 25 25 10 40
  :header-rows: 1

  * - Network Name
    - Address
    - VLAN
    - DHCP Scope
  * - Primary
    - 10.21.\ *XYZ*\ .1/25
    - 0
    - 10.21.\ *XYZ*\ .50-10.21.\ *XYZ*\ .124
  * - Secondary
    - 10.21.\ *XYZ*\ .129/25
    - *XYZ1*
    - 10.21.\ *XYZ*\ .132-10.21.\ *XYZ*\ .253

Credentials
...........

.. note::

  The *<Cluster Password>* is unique to each cluster and will be provided by the leader of the Bootcamp.

.. list-table::
  :widths: 25 35 40
  :header-rows: 1

  * - Credential
    - Username
    - Password
  * - Prism Element
    - admin
    - *<Cluster Password>*
  * - Prism Central
    - admin
    - *<Cluster Password>*
  * - Controller VM
    - nutanix
    - *<Cluster Password>*
  * - Prism Central VM
    - nutanix
    - *<Cluster Password>*

Each cluster has a dedicated domain controller VM, **DC**, responsible for providing AD services for the **NTNXLAB.local** domain. The domain is populated with the following Users and Groups:

.. list-table::
  :widths: 25 35 40
  :header-rows: 1

  * - Group
    - Username(s)
    - Password
  * - Administrators
    - Administrator
    - nutanix/4u
  * - SSP Admins
    - adminuser01-adminuser25
    - nutanix/4u
  * - SSP Developers
    - devuser01-devuser25
    - nutanix/4u
  * - SSP Power Users
    - poweruser01-poweruser25
    - nutanix/4u
  * - SSP Basic Users
    - basicuser01-basicuser25
    - nutanix/4u

Access Instructions
+++++++++++++++++++

The Nutanix Hosted POC environment can be accessed a number of different ways:

Parallels VDI
.................

1) Login to https://xld-uswest1.nutanix.com (for PHX) or https://xld-useast1.nutanix.com (for RTP) using your supplied credentials
2) Select HTML5 (web browser) OR Install the Parallels Client
3) Select a desktop or application of your choice.

**Nutanix Employees** - Use your NUTANIXDC credentials

PHX
---
**Non-Employees** - **Username:** PHX-POCxxx-User01 (up to PHX-POCxxx-User20), **Password:** *<Provided by Instructor>*

RTP
---
**Non-Employees** - **Username:** RTP-POCxxx-User01 (up to RTP-POCxxx-User20), **Password:** *<Provided by Instructor>*

Employee Pulse Secure VPN
..........................

https://sslvpn.nutanix.com - Use your CORP credentials

Non-Employee Pulse Secure VPN
..............................

1) If client already installed skip to step 5
2) To download the client, login to https://xlv-uswest1nutanix.com or https://xlv-useast1.nutanix.com using the supplied user credentials
3) Download and install client
4) Logout of the Web UI
5) Open client and ADD a connection with the following details:

Type: Policy Secure (UAC) or Connection Server(VPN)
Name: X-Labs - PHX
Server URL: xlv-uswest1.nutanix.com

OR

Type: Policy Secure (UAC) or Connection Server(VPN)
Name: X-Labs - RTP
Server URL: xlv-useast1.nutanix.com

6) Once setup, login with the supplied credentials