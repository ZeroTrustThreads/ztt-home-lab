# Linux: Install GNOME Boxes

## Goal

Install GNOME Boxes from the Linux distribution's trusted package source and verify hardware virtualization support.

## Why GNOME Boxes?

GNOME Boxes provides a simple interface over QEMU, KVM, libvirt, and SPICE. It is designed to make common virtual-machine tasks approachable while still using Linux's native virtualization stack.

## 1. Check hardware virtualization

If Boxes is already installed, run:

```bash
gnome-boxes --checks
```

Hardware virtualization may be called Intel VT-x or AMD-V in UEFI/BIOS. If it is disabled, use documentation from the computer or motherboard manufacturer before changing firmware settings.

## 2. Install from the distribution

Prefer the graphical software center or official package repository for your Linux distribution. Search for **GNOME Boxes**, review the package source, and install it.

Package names and commands differ between Ubuntu, Fedora, Debian, and other distributions. The project intentionally avoids presenting one command as universal.

Examples of trusted sources include:

- The distribution's built-in software application
- The distribution's official package repositories
- The verified GNOME Boxes listing on Flathub, if Flatpak is already part of your system's trusted workflow

## 3. Open Boxes

Launch GNOME Boxes. Confirm that the collection view opens and provides a `+` control for creating a box.

## Checkpoint

Boxes opens successfully, and the virtualization check does not report a blocking problem.

Continue to [Create the Ubuntu Server VM](02-create-ubuntu-server-vm.md).

## Knowledge check

1. Which Linux distribution and package source did you use?
2. What role does KVM play?
3. Why is a distribution-specific source preferable to an unknown download site?

## Sources and further reading

- [GNOME Boxes help](https://help.gnome.org/gnome-boxes/index.html)
- [GNOME Boxes system requirements](https://help.gnome.org/gnome-boxes/system-requirements.html)
- [Using processor hardware virtualization](https://help.gnome.org/gnome-boxes/virtualization.html)
- [Technology used by Boxes](https://help.gnome.org/gnome-boxes/supported-protocols.html)
