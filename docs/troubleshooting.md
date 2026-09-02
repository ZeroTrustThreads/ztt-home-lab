# Troubleshooting

## The VM boots back into the installer

Shut down the VM, detach the Ubuntu ISO from its virtual removable drive, and start the VM again.

## The VM has no IP address

- Confirm that the virtual network device is enabled in UTM.
- Restart the VM.
- Run `ip address` again.
- Confirm that macOS itself has working network access.

## SSH reports “connection refused”

On Ubuntu, check the service:

```bash
sudo systemctl status ssh
```

If it is missing, install `openssh-server`. If it is stopped, start it with:

```bash
sudo systemctl enable --now ssh
```

## SSH times out

- Recheck the VM IP address with `hostname -I`.
- Confirm that the VM is running.
- Confirm that the Mac and VM networking mode allow local communication.
- Check whether a firewall rule is blocking TCP port 22.

## SSH warns that the host identification changed

This can happen after rebuilding a VM or reusing its IP address. Do not bypass the warning automatically. Confirm that the VM was intentionally rebuilt, then remove only the obsolete key entry identified in the warning.

## Ubuntu cannot find a package

Refresh the package index:

```bash
sudo apt update
```

Then check the package name and network connection before trying again.

## Still stuck?

Record:

- The step you were completing
- The exact command entered
- The complete error message
- Mac architecture
- UTM version
- Ubuntu version
- Relevant VM network settings

Remove passwords, tokens, public IP addresses, and other sensitive information before sharing diagnostic output.

## Sources and further reading

- [OpenSSH server on Ubuntu](https://documentation.ubuntu.com/server/how-to/security/openssh-server/)
- [Ubuntu firewall documentation](https://documentation.ubuntu.com/server/how-to/security/firewalls/index.html)
- [UTM documentation](https://docs.getutm.app/)
