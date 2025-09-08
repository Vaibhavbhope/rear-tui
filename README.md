# rear-tui

A menu-driven Text User Interface (TUI) for configuring and managing ReaR (Relax-and-Recover) disaster recovery on RHEL and compatible systems.
This script provides a guided menu for setting up OUTPUT, BACKUP, and related ReaR configuration parameters, stored in /etc/rear/rear-tui.conf.

## Overview

ReaR TUI provides an intuitive, menu-driven interface that simplifies the configuration and operation of ReaR. Instead of manually editing configuration files, users can configure all aspects of their backup and recovery setup through interactive menus.

## Features

### Main Operations
- **Create rescue media and backup the system** - Complete disaster recovery preparation
- **Create only backup** - Backup data without creating rescue media
- **Create rescue media only** - Create bootable rescue media without backup
- **Interactive configuration editor** - Menu-driven configuration management
- **View Current Configuration** - View Current Configuration of rear-tui

## Prerequisites

- **Root privileges** - Must be run as root or with sudo
- **ReaR installed** - Relax-and-Recover package must be installed
- **Whiptail** - Text-based dialog utility (usually part of `newt` package)

#### Installing Packages on RHEL/CentOS/Fedora:
```bash
sudo dnf install rear newt
# or
sudo yum install rear newt
```

## Installation of script

1. Clone or download all script files to a directory:
```bash
git clone <repository-url>
cd rear-tui
```

2. Make the main script executable:
```bash
chmod +x rear-tui.sh
```

⚠️ Important Note

Using the ReaR TUI helps simplify configuration, but **it does not guarantee that your
backup or recovery will succeed**.  

- Always verify that backups are being created correctly.  
- Perform regular restore tests in a safe environment.  
- Ensure storage, network paths, and boot media are available and tested.  

ReaR TUI is only a helper for configuration — the responsibility for testing
and validating disaster recovery remains with the system administrator.
