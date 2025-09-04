## Authors
- Vaibhav Bhope

# rear-tui

A menu-driven Text User Interface (TUI) for configuring and managing ReaR (Relax-and-Recover) disaster recovery RHEL systems.

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


