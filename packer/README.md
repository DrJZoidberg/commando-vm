
CommandoVM & HashiCorp's Packer
=============================

Welcome to the packer builder of CommandoVM - a fully automated installation of the customizable commandvm platform.

Requirements
------------

* a hypervisor ( below are current hypervisors )
  * [Virtualbox](https://www.virtualbox.org/wiki/Downloads)
* HashiCorp's [packer](https://www.packer.io/downloads)
* [packer provisioner windows update](https://github.com/rgl/packer-provisioner-windows-update)
* 60 GB Hard Drive
* 2 GB RAM

Recommended
-----------

* 80+ GB Hard Drive
* 4+ GB RAM

Instructions
============

Standard install
----------------

1. make sure you have all the [pre-reqs](#requirements).
2. Download the zip from [https://github.com/fireeye/commando-vm](https://github.com/fireeye/commando-vm).
3. Decompress the zip and cd into the [win10_1809 folder](/packer/win10_1809/).
4. run the following command: `packer build packer build win10_1809_virtualbox_iso_to_finish.json`.
   > if you don't have packer in you path, then you will have to specify the full path to the packer binary.
  
This will automate the whole process of creating the base vm, doing a windows installation, and then installing all the necessary CommandoVM components.

Custom install
--------------

<!--
TODO: I want to get @DrJZoidberg's commentary on what he thinks should go into here
-->

1. make sure you have all the [pre-reqs](#requirements).
2. Download the zip from [https://github.com/fireeye/commando-vm](https://github.com/fireeye/commando-vm) into your Downloads folder.
3. Decompress the zip and cd into the [win10_1809 folder](/packer/win10_1809/).
4. Modify any of the .json files to your pleasure.
5. run the following command: `packer build packer build win10_1809_virtualbox_iso_to_finish.json`.
