---
layout: post
title: "Introduction to Network Automation – Workshop Report"
date:   2019-06-05 10:35:23 -0400
---

The 2019 Introduction to Network Automation Workshop in Minneapolis was well attended with over 30 participants. The sessions covered a wide range of topics to provide a basic familiarity with technologies and practices relevant to network
automation.

The first day of this track was mostly lecture-style overviews.

  - Nick Grundler from the University of Michigan covered **choosing a database for managing config information**, and gave a demo of the NetBox application ([[slides]](https://docs.google.com/presentation/d/1XMDa7IxIQptDU5brS19a75e0f-            AxKPGpcvOlxDykTgk/edit?usp=sharing)).
  - Mark Tinberg from University of Wisconsin presented on **choosing an automation framework**, and led discussion on the relative strengths of Ansible and Salt ([[slides]](https://docs.google.com/presentation/d/                                  1aOlVdj9pSAROUfYAccOCUUTowCOOg3hN9GA10C2W290/edit#slide=id.p)).
  - James Ostrander from the University of Michigan presented on **using Git for source management**, covering issue tracking, merge requests, and code review ([[slides]](https://docs.google.com/presentation/d/1CZp_W-                              oJbnJhixbrA31o9lDiQLxWQ04spMqdVOce3Yo/edit?usp=sharing)).  James also lead a lab to give participants hands-on experience with these workflows ([[lab materials]](https://nacn-workshop.github.io/git-training/)).
  - Grover Browning from the GlobalNOC and Indiana University presented on **templating network device configuration**, and covered the jinja2 templating framework ([[slides]](https://drive.google.com/open?id=14pg54C-pe6N-Xz1zMYd4eaCGyp1ugKBK)).
  - AJ Ragusa from the GlobalNOC and Indiana University presented on **network configuration frameworks**, covering YANG and OpenConfig, as well as data management and other challenges ([[slides]](https://drive.google.com/open?                    id=10CCjb4psuSn7l5Atp3tvCFoEjnfDTk0M)).

The first day wrapped up with a group discussion about the challenges of providing training to network engineering and operations teams to spread the knowledge of these tools and practices, and getting buy in from those teams.

The morning of the second day was dedicated to a **network automation lab**. Kris Steinhoff from the University of Michigan facilitated this session. During this lab participants installed VirtualBox and Vagrant, and used these tools to configure an environment to run a virtual Arista EOS device. This environment was then used to apply automation techniques with Ansible. ([[lab materials]](https://nacn-workshop.github.io/network-automation-intro-lab-2019/) and [[git repository]](https://  github.com/nacn-workshop/network-automation-intro-lab-2019))

The participants enjoyed this track, calling out the sense of community and shared experience with other participants, and the value of the hands-on sections. Based on feedback, future versions of this track will provide more hands-on material,   and find ways to help participants do some technical preparation for labs in advance to allow more time for experimentation with the automation technologies.
