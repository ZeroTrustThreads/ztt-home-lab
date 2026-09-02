# 🖥️ Zero Trust Threads Cybersecurity Home Lab

Build a beginner-friendly cybersecurity lab using virtual machines, Ubuntu Server, networking, and containers.

This project guides you through each step while explaining what you are building, why it matters, and how to verify that it works.

---

## 📌 Project Status

**Current milestone:** Foundation — Ubuntu Server in UTM with SSH access

The initial release is being built around macOS and UTM. Additional platforms may be added as the project grows.

---

## 🎯 What You Will Build

```text
Mac
 └── UTM
      └── Ubuntu Server VM
           ├── Local user account
           ├── Network connection
           ├── SSH access
           └── Future security labs
```

The finished foundation gives you an isolated Linux environment where you can safely practice system administration and defensive security concepts.

---

## 📚 What You Will Learn

- What virtual machines are and why security learners use them
- How to create an Ubuntu Server virtual machine
- How CPU, memory, storage, and networking affect a VM
- Essential Linux navigation and administration
- How to find the VM's IP address
- How SSH provides remote command-line access
- How to validate and troubleshoot your lab
- How to take snapshots before experiments

---

## ✅ Before You Begin

You will need:

- A Mac capable of running UTM
- Enough free storage for UTM, an Ubuntu image, and the virtual machine
- An internet connection for downloads and updates
- Administrator access to your Mac
- Time to read each step instead of rushing through the setup

Keep the lab isolated from sensitive personal or work systems. Use only software and systems you own or are authorized to operate.

---

## 🚀 Start Here

Start with the [platform chooser](docs/platform-chooser.md), then follow the path for your computer:

| Host computer | Virtualization tool | Installation path |
|---|---|---|
| macOS | UTM | [Mac path](docs/01-install-utm.md) |
| Windows | VMware Workstation Pro | [Windows path](docs/windows/01-install-vmware-workstation.md) |
| Linux | GNOME Boxes/KVM | [Linux path](docs/linux/01-install-gnome-boxes.md) |

After Ubuntu is installed, everyone continues with the shared lessons:

1. [Complete first boot and updates](docs/03-first-boot.md)
2. [Connect with SSH](docs/04-connect-with-ssh.md)
3. [Validate the foundation](checklists/foundation-validation.md)
4. [Troubleshoot common problems](docs/troubleshooting.md)
5. [Review the glossary](docs/glossary.md)
6. [Complete the knowledge checks](docs/knowledge-checks.md)
7. [Document your work](checklists/lab-journal-template.md)

---

## 🧪 Learning Method

Every stage follows the Zero Trust Threads approach:

### 1. Learn

Understand the component and the security concept behind it.

### 2. Build

Configure the component in your own lab.

### 3. Validate

Confirm the result instead of assuming it worked.

### 4. Explain

Describe what happened, what could fail, and how you would investigate it.

---

## 🗺️ Roadmap

### Milestone 1 — Foundation

- [ ] Install UTM
- [ ] Create an Ubuntu Server VM
- [ ] Complete Ubuntu setup
- [ ] Update the operating system
- [ ] Identify the VM's network address
- [ ] Connect through SSH
- [ ] Complete the validation checklist

### Milestone 2 — Linux Fundamentals

- [ ] Navigate files and directories
- [ ] Manage users and groups
- [ ] Understand permissions
- [ ] Inspect processes and services
- [ ] Read system logs

### Milestone 3 — Containers

- [ ] Install Docker
- [ ] Run a first container
- [ ] Understand images, containers, ports, and volumes
- [ ] Apply basic container safety practices

### Milestone 4 — Defensive Security Labs

- [ ] System hardening
- [ ] Log analysis
- [ ] File integrity monitoring
- [ ] Network observation
- [ ] Safe break-and-fix exercises

Projects will be added when their instructions and validation steps are ready.

---

## 📖 Documentation and Sources

The guides cite official product documentation so learners can verify procedures and continue beyond the project. See [REFERENCES.md](REFERENCES.md) for the source catalog and maintenance policy.

Commands are paired with explanations, checkpoints, validation evidence, and questions. The goal is to understand the system rather than copy commands without context.

---

## ⚠️ Responsible Use

This project is intended for educational and defensive security purposes.

Only test systems, applications, networks, or environments that you own or have explicit authorization to test. Do not expose intentionally vulnerable services to the public internet.

You are responsible for using these materials legally and safely.

---

## 🤝 Contributing

Bug reports, documentation improvements, accessibility improvements, and beginner-focused suggestions are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md) before proposing a change.

---

## 🧵 Zero Trust Threads

**One concept. One project. Learn by doing.**

Cybersecurity • Linux • GRC • Defensive Security • Security Culture
