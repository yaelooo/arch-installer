<h1 align="center">
  <a href="https://www.archlinux.org">Archlinux</a> Installer
</h1>
<h4 align="center">Please read the <a href="https://wiki.archlinux.org/title/installation_guide">Arch Linux installation guide</a> before running this script.</h4>

![installation](https://raw.githubusercontent.com/yaelooo/arch-installer/main/.ignore/arch-installer.webp)

## To do

- [ ] Minimal script
- [ ] Add compatibility for MBR

## Prerequisites.

- Run on an arch-based system.
- Running script as root.
- An active internet connection.
- GPT as partition scheme

## Download the script.

> [!IMPORTANT]
> Install git, wget or curl to download the script

### With git.

```
git clone https://github.com/yaelooo/arch-installer
```

### With wget.

```
wget -O- https://github.com/yaelooo/arch-installer/tarball/master | tar xz
```

### With curl.

```
curl -L https://github.com/yaelooo/arch-installer/tarball/master | tar xz
```

## How to use.

Change to the directory and run the script

```
./recommended
```

> [!WARNING]
> The installation will format your disk, proceed carefully and save important information.

## This script configure the next steps:

### Recommended

- Resize cowspace / [reference](https://wiki.archlinux.org/title/archiso#Adjusting_the_size_of_the_root_file_system).
- [1.0](https://wiki.archlinux.org/title/archiso#Adjusting_the_size_of_the_root_file_system) Pre-installation.
  - [1.5](https://wiki.archlinux.org/title/installation_guide#Set_the_console_keyboard_layout_and_font) Set the console keyboard layout and font.
  - [1.8](https://wiki.archlinux.org/title/installation_guide#Update_the_system_clock) Update the system clock.
  - [1.9](https://wiki.archlinux.org/title/installation_guide#Partition_the_disks) Partition the disks.
  - [1.10](https://wiki.archlinux.org/title/installation_guide#Format_the_partitions) Format the partitions.
  - [1.11](https://wiki.archlinux.org/title/installation_guide#Mount_the_file_systems) Mount the file systems.
- [2.0](https://wiki.archlinux.org/title/installation_guide#Installation) Installation.
  - [2.1](https://wiki.archlinux.org/title/installation_guide#Select_the_mirrors) Select the mirrors.
  - [2.2](https://wiki.archlinux.org/title/installation_guide#Install_essential_packages) Install essential packages.
- [3.0](https://wiki.archlinux.org/title/installation_guide#Configure_the_system) Configure the system.
  - [3.1](https://wiki.archlinux.org/title/installation_guide#Fstab) Fstab.
  - [3.3](https://wiki.archlinux.org/title/installation_guide#Time) Time.
  - [3.4](https://wiki.archlinux.org/title/installation_guide#Localization) Localization.
  - [3.5](https://wiki.archlinux.org/title/installation_guide#Network_configuration) Network configuration.
  - [3.7](https://wiki.archlinux.org/title/installation_guide#Root_password) Root password.
  - [3.8](https://wiki.archlinux.org/title/installation_guide#Boot_loader) Boot loader.
- Some additional configurations.
  - Enable some services (NetworkManager, dhcpcd, systemd-timesyncd) / [reference](https://wiki.archlinux.org/title/systemd#Using_units).
  - Copy the new mirrorlist (if it was configured during installation).
  - Add a user and set passwd / [reference](https://wiki.archlinux.org/title/users_and_groups).
  - Install YAY / [reference](https://github.com/Jguer/yay).
- [4.0](https://wiki.archlinux.org/title/installation_guide#Reboot) Reboot.
  - Unmount partitions.
  - Reboot.
