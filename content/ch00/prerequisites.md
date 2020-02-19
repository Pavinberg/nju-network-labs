# Prerequisites

## Virtual Machine

We are providing you with a Ubuntu 18.04 (64-bit) VM image for this assignment. This image has Switchyard, Mininet and Wireshark installed so you do not need to worry about setting up the enviroment.

- You can find the VM image [here](https://box.nju.edu.cn/d/123a70ac8ff34595b18f/).
(user name: njucs - password: 123)
- You can learn more about importing a VM image in VirtualBox [here](https://docs.oracle.com/cd/E26217_01/E26796/html/qs-import-vm.html).

You are also free to use your favorite vitualization software for importing the image but you will most probably have to deal with the possible issues on yourself.

If you are a free soul and want to setup Switchyard in a different environment you are welcome to do that as well. You can find some useful information [here](../../appendix/environment-setup.md). This might or might not be useful for you depending on your environment.

## Python

Switchyard and Mininet is developed in python. So you need to program in python (though there are some methods to avoid using python). Python is a easy-learning language. If you are not familiar with it, here are some materials for you to get started.

- [廖雪峰的 Python 3 教程](https://www.liaoxuefeng.com/wiki/1016959663602400)
- [Python 教程](https://docs.python.org/zh-cn/3/tutorial/index.html)
- [Learn Python - Free Interactive Python Tutorial](https://www.learnpython.org/)

Our VM is python preinstalled so you can skip installing. Topics you need to know about python are listed here

- Python Interpreter
- Data Types (Important)
- Data Structures (Important)
- Flow Control (Important)
- Functions (Important)
- Modules
- Input and Output
- Errors and Exceptions
- Standard Library
- Virtual Environments and Packages (Important)

Except those topics marked as important, it is no need to read it carefully, just program as you learn. We expect that you will cost about 3 days on this if you haven't worked with python.

> [!NOTE]
> Python 3 is the main language you will use in Switchyard programming. But you need to know some difference between Python 3 and Python 2 though they are mostly the same. Because you may write some Mininet topology scripts using Python 2.

## Mininet

Mininet enables you to quickly create, interact with, customize and share a software defined network prototype, and provides a smooth path to running on hardware.

The most useful material is their website. Here is the [Mininet Walkthrough](http://mininet.org/walkthrough/). It is better to go through this manual. Because we have not given you the whole network image to you right now, there must be something you do not understand yet. But don not worry, we will have a small practice of Mininet in our manual.

We expect that you will cost 2 days on this.

## Wireshark

Wireshark is the world’s foremost and widely-used network protocol analyzer. It lets you see what’s happening on your network at a microscopic level and is the de facto (and often de jure) standard across many commercial and non-profit enterprises, government agencies, and educational institutions.

You will use it to inspect your network setting up by Mininet, and test the function of your device written in Switchyard. We also have a small practice of Wireshark in our manual.

[Wireshark User’s Guide](https://www.wireshark.org/docs/wsug_html/) is a verbose document about Wireshark but We **do not** recommend it. So sometimes the offical document is hard for user to get started. You can find many blogs writing about how to use Wireshark. Read them instead.

We expect that you will cost an afternoon on this.

## Switchyard

Switchyard is a framework for creating, testing, and experimenting with software implementations of networked systems such as Ethernet switches, IP routers, firewalls and middleboxes, and end-host protocol stacks. It is the framework targeting on teaching and used in Wiscosin University.

So we have this framework to do some network testing without multiple devices and a bunch of wires. [Switchyard documentation](https://jsommers.github.io/switchyard/index.html) is available here. And this is the document you read most often. In this lab we will combine Mininet, Wireshark and Swithyard together, as we said before.

We expect that you will cost 4 days on this. It is long but important.

## Git (Optional)

You can use Git to manage your projects with a clear editing history and we recommend using it. It is better to have your local repository synchronized with a remote backup on GitHub or some one else. The tutorial of Git is listed below.

- [廖雪峰的 Git 教程](https://www.liaoxuefeng.com/wiki/896043488029600)

We expect that you will cost 2 days on this.