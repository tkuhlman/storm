Description
===========
Installs Twitter's Storm distributed computation platform.  Includes recipes for installing
both the Nimbus / Web UI component and the Supervisor component.

Requirements
============
* Ubuntu 10.04 / 12.04
* May function on other distributions, but has not been tested

* java cookbook
* runit cookbook

Attributes
==========

Usage
=====

This recipe relies on two setup components that need to be noted as they are not used
in many (or any) community cookbooks.

Cluster Setup:
- `node[:storm][:nimbus][:host]` with the fqdn/ip of the nimbus host
- `node[:storm][:zookeeper][:quorum]` with an array of fqdn/ips of the zookeeper hosts
