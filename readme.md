# A dockerized environment for building edgetx firmware and etc.

The [EdgeTX wiki](https://github.com/EdgeTX/edgetx/wiki) shows how to build firmware on different platforms. You will have to install all packages again and again if you are on different devices. You can build firmware using Cloud Builder, such as **GitPod**. But why don't I benifit from my 72 cores workmonster? So I created this docker image only for building custom edgetx firmware faster.

F.Y.I. I have 2 opensource radios: RadioMaster TX16S Mark 2 and FrSky Taranis X9D Plus (2015).

### How was this repo made?

Editor: vscode on macOS (M1)

Editor mode:  remote develpment using SSH

Remote PC: Ubuntu 22.04 on Intel X86_64 CPU

Remote PC preset: Install docker on ubuntu 22.04, then pull a Ubuntu 20.04 x86_64 image to local.

Network: With **Zerotier** installed on both macOS and Linux server, connect to the remote Linux server in VScode on macOS using virtual LAN IP such as 172.x.x.x (The Linux Server's zerotier LAN IP)

Docs are here <https://code.visualstudio.com/docs/remote/ssh>
