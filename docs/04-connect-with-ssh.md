# Connect with SSH

## Goal

Open an encrypted terminal session from the Mac to the Ubuntu Server VM.

## 1. Confirm the SSH service

In the Ubuntu VM, run:

```bash
sudo systemctl status ssh
```

The service should show `active (running)`. Press `q` to leave the status view.

If SSH was not installed during Ubuntu setup:

```bash
sudo apt update
sudo apt install openssh-server
sudo systemctl enable --now ssh
```

## 2. Find the VM address

```bash
hostname -I
```

Use the private network address shown. Ignore loopback addresses such as `127.0.0.1`.

## 3. Connect from the Mac

Open Terminal on the Mac and run:

```bash
ssh YOUR_USERNAME@VM_IP_ADDRESS
```

Replace both placeholders with the Ubuntu username and VM address.

On the first connection, SSH asks whether you trust the host key. Confirm that you are connecting to the expected VM before accepting it. Then enter the Ubuntu account password.

## 4. Validate the session

Run:

```bash
whoami
hostname
```

The commands should identify the Ubuntu user and VM, not the Mac.

Exit the session:

```bash
exit
```

## Next improvement

Password authentication is acceptable for the initial local lab. A later exercise will introduce SSH keys and explain when password authentication should be disabled.

Complete the [Foundation Validation Checklist](../checklists/foundation-validation.md).

## Knowledge check

1. What does the SSH host key identify?
2. Why should an unexpected changed-host-key warning be investigated?
3. How did `whoami` and `hostname` prove which computer ran the commands?

## Sources and further reading

- [OpenSSH server on Ubuntu](https://documentation.ubuntu.com/server/how-to/security/openssh-server/)
- [Ubuntu firewall documentation](https://documentation.ubuntu.com/server/how-to/security/firewalls/index.html)
