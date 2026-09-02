# Choose Your Host Platform

The **host** is the physical computer running the virtual machine. Choose one path below. All paths produce the same result: an Ubuntu Server VM that you can manage through SSH.

## Quick decision table

| Your computer | Recommended beginner tool | Continue with |
|---|---|---|
| Mac with Apple silicon or Intel | UTM | [Install UTM](01-install-utm.md) |
| Windows PC with an Intel or AMD processor | VMware Workstation Pro | [Install VMware Workstation](windows/01-install-vmware-workstation.md) |
| Linux computer with hardware virtualization | GNOME Boxes | [Install GNOME Boxes](linux/01-install-gnome-boxes.md) |

## Why the instructions use different tools

The underlying ideas are the same—virtual CPU, memory, disk, installation media, and networking—but each host platform offers different beginner-friendly software. Learning the concepts makes it easier to use another virtualization product later.

## Architecture check

The guest image must be compatible with the virtual machine architecture.

- Most Intel and AMD Windows/Linux computers use the Ubuntu **AMD64** image.
- Apple silicon Macs use the Ubuntu **ARM64** image with UTM virtualization.
- Intel Macs use the Ubuntu **AMD64** image.
- Windows on ARM and less common Linux architectures require extra compatibility checks and are not yet validated by this project.

If you do not know your architecture, use the platform-specific preflight steps before downloading Ubuntu.

## Resource guidance

The starter configuration is 2 CPU cores, 4 GB RAM, and 25 GB storage. Treat this as a starting point. A host with limited resources may use less, but installation and updates will be slower.

Do not allocate all host memory or CPU capacity to the VM. The host operating system must remain usable.

## Shared lessons

After installing Ubuntu, every learner continues with:

1. [First boot and updates](03-first-boot.md)
2. [Connect with SSH](04-connect-with-ssh.md)
3. [Foundation validation](../checklists/foundation-validation.md)
4. [Knowledge checks](knowledge-checks.md)

## Knowledge check

Explain which host, virtualization tool, and Ubuntu architecture you selected and why they are compatible.
