# Glossary

## Architecture

The instruction set used by a processor. Apple silicon Macs use ARM64; Intel Macs use AMD64/x86-64. A guest image and virtualization configuration must be compatible with the host architecture.

## Guest

The operating system running inside a virtual machine. Ubuntu Server is the guest in this lab.

## Host

The physical computer and operating system running the virtualization software. The Mac is the host in this lab.

## Hypervisor

Software or a system framework that creates and manages virtual machines. UTM provides the interface used to manage the lab VM.

## IP address

A numerical address used to identify a network interface. The lab uses a private IP address to connect from the Mac to Ubuntu.

## ISO image

A file containing the contents of installation media. The Ubuntu Server ISO is attached to the VM to install the operating system.

## LTS

Long Term Support. Ubuntu LTS releases receive a longer standard support period than interim releases and are preferred for this learning environment.

## Port

A numbered network endpoint used by an application or service. SSH normally listens on TCP port 22.

## Snapshot

A saved VM state or disk checkpoint used to recover after a lab mistake. A snapshot is useful but does not replace a separate backup.

## SSH

Secure Shell, an encrypted protocol for remote login and command execution.

## Virtual machine (VM)

A software-defined computer with virtual CPU, memory, storage, and network devices.

## Virtualization

Running a guest built for the same processor architecture as the host with hardware assistance. This is generally faster than emulating another architecture.
