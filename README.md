#  Volatility3 Memory Analysis Framework Installation Lab

Volatility is an open-source memory forensics framework used to analyze memory dumps. It supports identifying the OS profile, listing active processes, visualizing parent-child relationships to detect suspicious behavior, identifying hidden or unlinked processes often caused by malware, inspecting network connections, detecting injected code, and even dumping process memory.

This guide documents how I installed [Volatility3](https://github.com/volatilityfoundation/volatility3) on my homelab running Kali Linux.

For my hands-on analysis, I'll be using [MemLabs Lab 1 - Beginner's Luck](https://github.com/stuxnet999/MemLabs/tree/master/Lab%201), showcasing techniques learned from the [TryHackMe Volatility Module](https://tryhackme.com/room/volatility) in a separate project series.

## System Setup

### Installing System Dependencies

Install essential packages required for memory analysis:

```bash
sudo apt update && sudo apt install -y build-essential git libdistorm3-dev yara libraw1394-11 libcapstone-dev capstone-tool tzdata
```

📸 [INSTALL_SYSTEM_DEPENDENCIES.jpeg](https://github.com/Jones-Waka/Volatility/blob/screenshots/INSTALL%20SYSTEM%20DEPENDENCIES.JPG)): Demonstrates successful installation of required system packages.

---

###  Installing Python3 & pip

Ensure Python3 and pip are available for Volatility execution:

```bash
sudo apt install -y python3 python3-dev python3-pip python3-setuptools python3-wheel
```

📸 [INSTALL_PYTHON3_AND_PIP.jpeg](https://github.com/Jones-Waka/Volatility/blob/screenshots/INSTALL%20PYTHON3%20%26%20PIP.JPG): Python3 and pip installation on Kali Linux.

---

###  Clone and Launch Volatility3

Download the Volatility3 repository and run a basic check:

```bash
git clone https://github.com/volatilityfoundation/volatility3.git
cd volatility3
python3 vol.py --info
```

📸 [CLONE_VOLATILITY3_REPO.jpeg](https://github.com/Jones-Waka/Volatility/blob/screenshots/CLONE%20AND%20INSTALL%20VOLATILITY%203.JPG): Shows the GitHub repository clone and verification of Volatility3 capabilities.

##  Reference

[Volatility Foundaton Github Page](https://github.com/volatilityfoundation/volatility/wiki/installation)

[Tryhackme Volatility Module](https://tryhackme.com/room/volatility)

##  GitHub Stats  

![Jones's GitHub Stats](https://github-readme-stats.vercel.app/api?username=Jones-Waka&show_icons=true&theme=radical) 
