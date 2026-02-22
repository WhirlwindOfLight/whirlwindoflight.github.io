layout: page
title: "Projects"
permalink: /projects
## HardwareVNC
A program designed to help control VMs created with [GPU passthrough](https://wiki.archlinux.org/title/PCI_passthrough_via_OVMF), since those VMs can't easily use traditional remoting solutions that involve attaching a server directly to a virtual GPU. As the name implies, this program works by using hardware to control the VM, by using a capture card connected to the passed-through GPU to see the display, and by using a TCP connection to [another program](https://github.com/WhirlwindOfLight/VM-Controller) to control the keyboard and mouse.

## VM-Controller
A program designed to create virtual input devices (to control physical or virtual machines) that take TCP input and convert it into keyboard and mouse signals. It was originally designed to respond to packets sent from [HardwareVNC](https://github.com/WhirlwindOfLight/HardwareVNC), but it can also be used in combination with [VM-HardwareForwarder](https://github.com/WhirlwindOfLight/VM-HardwareForwarder) to forward physical keyboard and mouse signals from one machine to another.

## VM-HardwareForwarder
A program designed to forward physical keyboard and mouse input to a machine running [VM-Controller](https://github.com/WhirlwindOfLight/VM-Controller). It was originally designed to use physical hardware to control VMs managed by [HardwareVNC](https://github.com/WhirlwindOfLight/HardwareVNC), but it can also be used to share a keyboard and mouse between two physical machines.
