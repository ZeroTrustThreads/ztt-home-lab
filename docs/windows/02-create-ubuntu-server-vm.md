# Windows: Create the Ubuntu Server VM

## Goal

Create an Ubuntu Server VM in VMware Workstation Pro using settings suitable for a beginner lab.

## 1. Download Ubuntu Server

Download a current Ubuntu Server LTS **AMD64** ISO from <https://ubuntu.com/download/server> for a standard Intel or AMD Windows PC.

An LTS release is preferred for stability and its longer support period.

## 2. Create the VM

1. Open VMware Workstation Pro.
2. Choose **Create a New Virtual Machine**.
3. Select the typical or recommended configuration when offered.
4. Select the downloaded Ubuntu Server ISO.
5. Name the VM `ztt-ubuntu-server`.
6. Choose a storage location with sufficient free space.
7. Start with approximately:
   - 2 processor cores
   - 4 GB memory
   - 25 GB virtual disk
8. Use the default NAT network for the initial lab.
9. Review the summary before creating the VM.

Interface labels can vary by Workstation release. Focus on the purpose of each resource rather than matching screenshots blindly.

## 3. Install Ubuntu

1. Start the VM and follow the Ubuntu Server installer.
2. Confirm that the virtual network interface receives an address.
3. Use the default storage layout unless you are intentionally studying partitioning.
4. Create a non-root administrator account with a unique password.
5. Select **OpenSSH server** when offered.
6. Complete installation and reboot.
7. Disconnect the ISO if the installer starts again.

## Checkpoint

Ubuntu boots to a login prompt and accepts the account created during installation.

Continue to [First Boot and Updates](../03-first-boot.md).

## Knowledge check

1. What does NAT allow the VM to do?
2. Why should the host retain some CPU and memory?
3. Why did you select the AMD64 Ubuntu image?

## Sources and further reading

- [Download Ubuntu Server](https://ubuntu.com/download/server)
- [Ubuntu Server installation](https://documentation.ubuntu.com/server/how-to/installation/index.html)
- [Ubuntu Server reference](https://documentation.ubuntu.com/server/reference/index.html)
