## Work in progress
---
layout: post
title:  "UofM North Campus Data Center"
date:   2019-05-08 12:00:00 -0400
---

##Overview
The University of Michigan deployed a new data center in Fall of 2018. As a
greenfield deployment we were able to standardize around a contemporary
spine/leaf architecture using EVPN/VXLAN.  One of our high-level goals for this
data center was to manage the network device configuration using an external
source of authority.

##Automation Details
We decided to use Netbox as our external source of authority, and we the Salt
automation framework to extract, render, and deliver configuration to the
devices. To facilitate this we wrote a netbox salt module that was contributed
back to the Salt project and included in the Fluorine release in February 2019.

![](/assets/2019-05-08_umich-ncdc-automation-workflow.png)

One of the first issues we bumped into was that while Netbox is covered a lot
of our use cases, there was still pieces of configuration data that could not
be expressed using Netbox’s data model.  For these situations, we chose to use
YAML files stored in our internal Gitlab instance.  One of the reasons we chose
Salt for our framework was the ease at which it is able to aggregate multiple
data sources together and present a single data structure(python dictionary) to
the device, which can then be easily referenced in further tasks, such as
templating.
