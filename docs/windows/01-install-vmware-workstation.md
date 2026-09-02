# Windows: Install VMware Workstation Pro

## Goal

Install VMware Workstation Pro from Broadcom's official download portal and confirm that the host is ready to create an Ubuntu VM.

## Supported path

This beginner path targets a standard 64-bit Windows PC with an Intel or AMD processor. Windows on ARM is not yet validated in this project.

## 1. Check the Windows system

1. Open **Settings → System → About**.
2. Record the processor and system type.
3. Confirm that enough memory and free storage remain for the host and VM.
4. Open **Task Manager → Performance → CPU** and check whether **Virtualization** shows as enabled.

If virtualization is disabled, the setting may need to be enabled in the computer's UEFI/BIOS. Names vary by manufacturer and may include Intel Virtualization Technology, VT-x, or AMD-V. Follow the computer manufacturer's documentation rather than changing unrelated firmware settings.

## 2. Download VMware Workstation Pro

1. Go to the [Broadcom Support Portal](https://support.broadcom.com/).
2. Sign in or create a basic account.
3. Open **My Downloads → Free Software Downloads**.
4. Search for **VMware Workstation Pro**.
5. Select the current Windows release.
6. Review and accept the applicable terms.
7. Download the installer.

Broadcom's download workflow and product naming may change. Use the current official instructions linked below if the menus differ.

## 3. Install

1. Verify that the installer came from Broadcom.
2. Launch it and read each prompt.
3. Keep the default components unless you understand why a change is needed.
4. Reboot Windows if requested.
5. Open VMware Workstation Pro and confirm that its home screen appears.

## Checkpoint

VMware Workstation opens and offers an option to create a new virtual machine.

Continue to [Create the Ubuntu Server VM](02-create-ubuntu-server-vm.md).

## Knowledge check

1. Where did you obtain the installer?
2. What evidence shows hardware virtualization is enabled?
3. Why should virtualization settings be changed using manufacturer guidance?

## Sources and further reading

- [Broadcom: Downloading free software](https://knowledge.broadcom.com/external/article/397417/downloading-free-software-from-the-broad.html)
- [Broadcom: Download VMware Workstation Pro](https://knowledge.broadcom.com/external/article/344595/downloading-vmware-workstation-pro.html)
- [Broadcom: Desktop hypervisor downloads](https://knowledge.broadcom.com/external/article/368734/download-desktop-hypervisor-workstation.html)
