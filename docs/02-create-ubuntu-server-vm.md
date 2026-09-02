# Create the Ubuntu Server VM

## Goal

Download Ubuntu Server from an official source and create a VM with reasonable starter resources.

## 1. Identify your Mac architecture

Open **Apple menu → About This Mac**.

- Apple silicon Macs use an ARM64 Ubuntu image.
- Intel Macs use an AMD64 Ubuntu image.

The image architecture must match the VM configuration.

## 2. Download Ubuntu Server

Download a current Ubuntu Server LTS image from <https://ubuntu.com/download/server>.

Prefer an LTS release for a stable learning environment. Keep the downloaded ISO until installation succeeds.

## 3. Create the VM in UTM

1. Select **Create a New Virtual Machine**.
2. Choose **Virtualize** when your Ubuntu image matches the Mac architecture.
3. Choose **Linux**.
4. Select the downloaded Ubuntu Server ISO as the boot image.
5. Assign starter resources based on what your Mac can comfortably support:
   - 2 CPU cores
   - 4 GB memory
   - 25 GB storage
6. Keep shared directories disabled initially. They can be added later when their security implications are understood.
7. Name the VM something clear, such as `ztt-ubuntu-server`.
8. Save the configuration and start the VM.

Do not allocate so many resources that macOS becomes unstable. These values are a starting point, not a universal requirement.

## 4. Install Ubuntu Server

Follow the Ubuntu installer:

1. Select your language and keyboard layout.
2. Confirm that a network interface receives an address.
3. Use the default storage layout unless you intentionally want to study disk partitioning.
4. Create a non-root administrator account.
5. Use a unique password that is not reused elsewhere.
6. Select the option to install **OpenSSH server** when offered.
7. Complete the installation and reboot.
8. Detach the installer ISO if the VM starts the installer again.

## Checkpoint

Ubuntu should boot to a login prompt and accept the account created during installation.

Continue to [First Boot](03-first-boot.md).

## Knowledge check

1. Which architecture does your Mac use?
2. Which Ubuntu image did you choose, and why is it compatible?
3. What tradeoff did you make when assigning memory and CPU cores?

## Sources and further reading

- [View About settings on Mac](https://support.apple.com/guide/mac-help/view-about-settings-mchlea7173f3/mac)
- [Download Ubuntu Server](https://ubuntu.com/download/server)
- [Ubuntu Server installation](https://documentation.ubuntu.com/server/how-to/installation/index.html)
- [Ubuntu Server reference and system requirements](https://documentation.ubuntu.com/server/reference/index.html)
