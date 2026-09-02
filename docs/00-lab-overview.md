# Lab Overview

## Goal

Create an Ubuntu Server virtual machine on a Mac and manage it remotely through SSH.

## What each component does

- **Mac:** The physical host computer.
- **UTM:** The virtualization application that creates and runs the virtual machine.
- **Ubuntu Server:** The guest operating system used for Linux and security practice.
- **SSH:** The encrypted protocol used to open a remote terminal session to the VM.

## Why use a virtual machine?

A virtual machine separates the learning environment from the host operating system. You can experiment, take snapshots, recover from mistakes, and rebuild without dedicating another physical computer.

Isolation is useful, but it is not absolute protection. Avoid storing sensitive information in the lab, do not bridge it to networks you do not control, and do not expose lab services directly to the internet.

## Definition of done

The foundation is complete when:

1. Ubuntu Server boots successfully in UTM.
2. The VM has network access.
3. The operating system is updated.
4. The SSH service is running.
5. You can connect from the Mac terminal using the VM's local IP address.
6. You record the configuration and create a clean snapshot.

Continue to [Install UTM](01-install-utm.md).

## Knowledge check

Before continuing, explain the difference between the host, guest, virtualization application, and SSH connection. Review the definitions in the [glossary](glossary.md) if needed.

## Sources and further reading

- [UTM documentation](https://docs.getutm.app/)
- [Ubuntu Server installation documentation](https://documentation.ubuntu.com/server/how-to/installation/index.html)
