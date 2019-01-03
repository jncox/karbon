.. title:: Nutanix Era Labs

.. toctree::
  :maxdepth: 2
  :caption: Karbon Tech Summit 2019 Lab
  :name: _karbon_tech_summit_2019_lab
  :hidden:

  karbon/karbon

.. toctree::
  :maxdepth: 2
  :caption: Pre-Requirements
  :name: _prerequirements
  :hidden:

  appendix/install_wget
  appendix/install_kubectl

.. toctree::
  :maxdepth: 2
  :caption: Karbon Labs
  :name: _karbon_labs
  :hidden:

  karbon_enable_and_images/karbon_enable_and_images
  karbon_create_cluster/karbon_create_cluster
  karbon_deploy_application/karbon_deploy_application
  karbon_delete_application/karbon_delete_application

.. toctree::
  :maxdepth: 2
  :caption: Appendix
  :name: _appendix
  :hidden:

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
  - AOS & PC 5.10.x

Access Instructions
+++++++++++++++++++

The Nutanix Hosted POC environment can be accessed a number of different ways:

Citrix XenDesktop
.................

https://citrixready.nutanix.com - *Accessible via the Citrix Receiver client or HTML5*

**Nutanix Employees** - Use your NUTANIXDC credentials

**Non-Employees** - **Username:** POCxxx-User01 (up to POCxxx-User20), **Password:** *<Provided by Instructor>*

Employee Pulse Secure VPN
..........................

https://sslvpn.nutanix.com - Use your CORP credentials

Non-Employee Pulse Secure VPN
..............................

https://lab-vpn.nutanix.com - **Username:** POCxxx-User01 (up to POCxxx-User20), **Password:** *<Provided by Instructor>*

Under **Client Application Sessions**, click **Start** to the right of **Pulse Secure** to download the client.

Install and open **Pulse Secure**.

Add a connection:

- **Type** - Policy Secure (UAC) or Connection Server
- **Name** - HPOC VPN
- **Server URL** - lab-vpn.nutanix.com
