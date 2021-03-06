# Lab 6: Reliable Communication

## Overview

In your final assignment you are going to build a reliable communication library in Switchyard that will consist of 3 agents. At a high level, a **blaster** will send data packets to a **blastee** through a **middlebox**. As you should all know by now, IP only offers a best-effort service of delivering packets between hosts. This means all sorts of bad things can happen to your packets once they are in the network: they can get lost, arbitrarily delayed or duplicated. Your communication library will provide additional delivery guarantees by implementing some basic mechanisms at the blaster and blastee. Let's move on to the details.

Lab-6 assignment in Github Classroom: [https://classroom.github.com/a/0zPMNWtr](https://classroom.github.com/a/0zPMNWtr)

## Your Tasks

In the source directory for this exercise, you can find the starter files: `middlebox.py`, `blastee.py` and `blaster.py`.

Your reliable communication library will implement the following features to provide additional guarantees: 1. ACK mechanism on blastee for each successfully received packet 2. A fixed-size sliding window on blaster 3. Coarse timeouts on blaster to resend non-ACK'd packets

Further details will be discussed in each Task.

{% hint style="info" %}
The sentences marked with ✅ are related to the content of your report. Please pay attention.
{% endhint %}

### Task 1: Preparation

Initiate your project with our template.

[Start the task here](preparation.md)

### Task 2: Middlebox

Implement the features of middlebox.

[Start the task here](middlebox.md)

### Task 3: Blastee

Implement the features of blastee.

[Start the task here](blastee.md)

### Task 4: Blaster

Implement the features of blaster.

[Start the task here](blaster.md)

### Task 5: Running your code

Make sure that your blaster, blastee and middlebox function correctly.

[Start the task here](deploy.md)

{% hint style="warning" %}
Please carefully read the [FAQ](faq.md) section, for more specific details regarding the implementations.
{% endhint %}

## Handing it in

Create a directory named `report/` in your repository and place your report, capture files and other materials in it.

### Report

We will provide a template of your lab assignment report [here](https://box.nju.edu.cn/d/f334d2c3bd4446b68003/). You need to submit the report in your repository named `<student ID><name>_lab_6.pdf`. The format of your report should be PDF. An example is `123456789拾佰仟_lab_6.pdf`.

### Capture file

The capture file's name should be `lab_6.pcapng` or `lab_6.pcap`.

### Submit to GitHub Classroom

Finally, the directory should be in this structure:

```text
.
├── README.md
├── blastee.py
├── blastee_params.txt
├── blaster.py
├── blaster_params.txt
├── middlebox.py
├── middlebox_params.txt
├── report
│   ├── 123456789拾佰仟_lab_6.pdf
│   └── lab_6.pcap
└── start_mininet.py
```

Commit the change.

{% hint style="warning" %}
**Only** commit your **source code** to your local repository. If there are some generated files that are not source code, ignore them by adding them in the file `.gitignore`.
{% endhint %}

After you’ve committed you final codes and report, push the repository to GitHub by inputing command:

```text
$ git push
```

After a few seconds, you can see the changes on your repository web page, which means you have handed in successfully.

