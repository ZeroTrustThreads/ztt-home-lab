# Linux: Create the Ubuntu Server VM

## Goal

Create an Ubuntu Server VM in GNOME Boxes and complete the base installation.

## 1. Identify the host architecture

Run:

```bash
uname -m
```

Common results:

- `x86_64` generally uses the Ubuntu AMD64 image.
- `aarch64` or `arm64` generally uses the Ubuntu ARM64 image.

Confirm support for the chosen image and virtualization stack before continuing.

## 2. Download Ubuntu Server

Download a current Ubuntu Server LTS image from <https://ubuntu.com/download/server> that matches the VM architecture.

## 3. Create the box

1. Open GNOME Boxes.
2. Click `+` to create a box.
3. Select the downloaded ISO file.
4. Continue to **Review and Create**.
5. Adjust resources when needed. A starting point is:
   - 2 CPU cores
   - 4 GB memory
   - 25 GB maximum storage
6. Create and start the VM.

Boxes may recommend resources automatically. Confirm that the Linux host retains enough memory and CPU capacity to remain responsive.

## 4. Install Ubuntu

1. Follow the Ubuntu Server installer.
2. Confirm that the network interface receives an address.
3. Use the default storage layout unless studying partitioning.
4. Create a non-root administrator account with a unique password.
5. Select **OpenSSH server** when offered.
6. Complete installation and reboot.
7. Remove the ISO from the virtual CD/DVD device if installation starts again.

## Checkpoint

Ubuntu boots to a login prompt and accepts the account created during installation.

Continue to [First Boot and Updates](../03-first-boot.md).

## Knowledge check

1. What architecture did `uname -m` report?
2. How does KVM differ from the Boxes interface?
3. Why is maximum virtual disk size not always the same as current host disk usage?

## Sources and further reading

- [Create a box](https://help.gnome.org/gnome-boxes/create.html)
- [GNOME Boxes interface and resources](https://help.gnome.org/gnome-boxes/interface.html)
- [GNOME Boxes system requirements](https://help.gnome.org/gnome-boxes/system-requirements.html)
- [Download Ubuntu Server](https://ubuntu.com/download/server)
- [Ubuntu Server installation](https://documentation.ubuntu.com/server/how-to/installation/index.html)
