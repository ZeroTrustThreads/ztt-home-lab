# Knowledge Checks

Answer these in your own words. The goal is understanding, not memorization.

## Lab design

1. What is the difference between the host and guest systems?
2. Why is a VM useful for cybersecurity learning?
3. Why does a VM reduce risk without providing perfect isolation?
4. What is the difference between virtualization and emulation?

## Platform selection

1. Why does the recommended virtualization application differ by host operating system?
2. How did you identify your processor architecture?
3. Why must guest and VM architectures be compatible?
4. Which parts of the lab remain the same across macOS, Windows, and Linux?

## Ubuntu installation

1. Why must the Ubuntu image architecture match the VM configuration?
2. Why is an LTS release a sensible default for this lab?
3. Why should the lab administrator account use a unique password?
4. What happens if the installer ISO remains first in the boot order?

## Networking and SSH

1. What information does `ip address` show?
2. Why can `127.0.0.1` not be used to connect from the Mac to the VM?
3. What does the SSH host-key prompt protect against?
4. What is the difference between “connection refused” and a timeout?
5. Why should a changed-host-key warning be investigated before it is removed?

## Updates

1. What is the difference between `apt update` and `apt upgrade`?
2. Why should you read the proposed package changes before approving them?
3. Why might Ubuntu temporarily keep an update back?

## Practical challenge

Without looking at the instructions, demonstrate the following:

1. Start the VM.
2. Find its current IP address.
3. Confirm the SSH service is running.
4. Connect from the Mac.
5. Prove that the terminal session is on Ubuntu.
6. Exit cleanly.

Record the commands used and explain what each command proved.
