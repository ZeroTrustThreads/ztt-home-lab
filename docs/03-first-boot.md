# First Boot and Updates

## Goal

Verify the installed system, apply updates, and record basic system information.

## Sign in

Use the local account created during installation. Password characters do not appear while you type; this is normal on Linux terminals.

## Inspect the system

Run:

```bash
hostnamectl
```

Then inspect the network interfaces:

```bash
ip address
```

Record the hostname and the private IP address assigned to the VM. Private addresses commonly begin with `10.`, `172.16` through `172.31`, or `192.168.`.

## Apply updates

```bash
sudo apt update
sudo apt upgrade
```

Read the proposed changes before confirming them. Reboot if the update process indicates that a reboot is required:

```bash
sudo reboot
```

## Checkpoint

After rebooting, confirm that you can sign in and that `ip address` still shows an active network interface.

Continue to [Connect with SSH](04-connect-with-ssh.md).

## Knowledge check

1. What information does `hostnamectl` establish?
2. What is the difference between refreshing package information and installing available upgrades?
3. Why should proposed changes be reviewed before approval?

## Sources and further reading

- [APT upgrades and phased updates](https://documentation.ubuntu.com/server/explanation/software/about-apt-upgrade-and-phased-updates/)
- [Ubuntu release upgrade guidance](https://documentation.ubuntu.com/server/how-to/software/upgrade-your-release/)
