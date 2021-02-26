# Lab 5: Respond to ICMP

## Overview

This is the third stage in a series of exercises that have the ultimate
goal of creating an IPv4 router. The basic functions of an Internet
router are to:

1.  Respond to ARP (address resolution protocol) requests for addresses
    that are assigned to interfaces on the router. (Remember that the
    purpose of ARP is to obtain the Ethernet MAC address associated with
    an IP address so that an Ethernet frame can be sent to another host
    over the link layer.)
2.  Receive and forward packets that arrive on links and are destined to
    other hosts. Part of the forwarding process is to perform address
    lookups ("longest prefix match" lookups) in the forwarding table. We
    will just use "static" routing in our router rather than implement a
    dynamic routing protocol like RIP or OSPF.
3.  Make ARP requests for IP addresses that have no known Ethernet MAC
    address. A router will often have to send packets to other hosts,
    and needs Ethernet MAC addresses to do so.
4.  Respond to ICMP messages like echo requests ("pings").
5.  Generate ICMP error messages when necessary, such as when an IP
    packet's TTL (time to live) value has been decremented to zero.

The goal of this stage of the project is to accomplish items **#4** and **#5**
above. When you're done with this project, you will have a fully
functioning Internet router. 

## Your Tasks

After the efforts of Lab 3 and Lab 4, you have implemented part of the functions of the router, including the response to ARP and the forwarding of packets. Next, you need to continue to improve your router in the `myrouter.py` so that it can respond to ICMP messages.

The main task for this exercise is to modify the Router class to do the following:

{% hint style="info" %}
The sentences marked with ✅ are related to the content of your report. Please pay attention.
{% endhint %}

### Task 1: Preparation

Initiate your project with our template.

[Start the task here](preparation.md)

### Task 2: Responding to ICMP echo requests

Respond to ICMP messages like echo requests ("pings").

[Start the task here](respond-ICMP.md)

### Task 3: Generating ICMP error messages

Generate ICMP error messages when necessary.

[Start the task here](generate-error-messages.md)

## Handing it in

### Report

We will provide a template of your lab assignment report [here](https://box.nju.edu.cn/d/123a70ac8ff34595b18f/). You need to submit the report in your repository named `<学号><姓名>_lab_5`. The format of your report can be Microsoft Doc or PDF. An example is `123456789拾佰仟_lab_5.pdf`.

### Submit to NJU GitLab

To submit your work, you need to do the following things.

1. Modify your code and complete your report.

2. When you have done your work, put your report and code in the folder `lab_5` then commit them. Tag the commit named `<学号/lab_5>` which you want to submit. An example is `123456789/lab_5`. Finally your project will look like

   ```
   switchyard
     ├─docs/
     ├─.../
   + ├─lab_5/
   + │ ├─123456789拾佰仟_lab_5.pdf
   + │ ├─myrouter.py
   + │ ├─forwarding_table.txt
     │ ├─...
   + │ └─start_mininet.py
     ├─.gitignore
     └─...
   ```
  {% hint style="warning" %}
  The file names in your submission have to **exactly** match the file names above. Otherwise, you will lose points!
  {% endhint %}

3. Submit your work by pushing your local repository to your remote repository **with your tags** by running the command `git push origin --tags`.

  {% hint style="warning" %}
  **Only** commit your **source code** to your local repository. If there are some generated files that are not source code, ignore them by adding them in the file `.gitignore`.
  {% endhint %}