# Linux File System Terms

<kbd>![image](img/linux_filesystem.png)</kbd>

## General Concepts

- **File System**: The structure used by Linux to store and organize files.
- **Mounting**: The process of attaching a file system to a directory so it can be accessed.
- **Partition**: A section of a storage device that acts as an independent file system.
- **Inode**: A data structure that stores metadata about a file (size, permissions, owner, timestamps, etc.).
- **File Descriptor**: A number assigned to open files and used by the system to reference them.

## File System Hierarchy

- **Root Directory (`/`)**: The top-level directory that contains all other directories and files.
- **Important Directories**:
  - `/bin` → Essential binary files (commands like `ls`, `cp`, `mkdir`).
  - `/sbin` → System binaries (administrative commands like `fdisk`, `reboot`).
  - `/etc` → System configuration files.
  - `/home` → Home directories for users.
  - `/root` → Home directory of the root user.
  - `/var` → Variable data (logs, temporary files, cache).
  - `/tmp` → Temporary files (cleared on reboot).
  - `/usr` → User-related system files (additional applications, libraries).
  - `/dev` → Device files (representing hardware like disks, printers).
  - `/proc` → Virtual file system containing system and process information.
  - `/sys` → Virtual file system that exposes kernel and hardware details.
  - `/mnt` → Temporary mount point for external devices.
  - `/media` → Mount point for removable media like USB drives.
  - `/opt` → Optional software installed outside the package manager.
  - `/boot` → Files related to booting the system (e.g., Linux kernel, GRUB).

## Common File System Types

- **ext4 (Fourth Extended File System)**: Default and most common file system in Linux.
- **ext3 (Third Extended File System)**: Older version of ext4 with journaling support.
- **XFS**: High-performance file system used for large-scale data storage.
- **Btrfs (B-Tree File System)**: Advanced file system with snapshot and compression features.
- **ZFS (Zettabyte File System)**: High-resilience file system with data integrity features.
- **FAT32**: Compatible with Windows and Linux but lacks modern security features.
- **NTFS (New Technology File System)**: Windows file system, supported in Linux via `ntfs-3g`.
- **ISO 9660**: File system for optical discs (CD/DVD).
- **tmpfs**: Temporary file system stored in RAM, used for `/tmp`.

## File System Operations

- **Mount (`mount`)**: Attach a file system to a directory.
- **Unmount (`umount`)**: Detach a file system.
- **Check Disk (`fsck`)**: Check and repair file system errors.
- **Create File System (`mkfs`)**: Format a partition with a specific file system.
- **List Partitions (`lsblk`, `fdisk -l`)**: Display storage devices and partitions.
- **Resize File System (`resize2fs`, `xfs_growfs`)**: Change the size of a file system.
- **Check Disk Usage**:
  - `df` → Show disk space usage.
  - `du` → Show directory/file size.

## File Permissions & Ownership

- **Permissions (`chmod`)**:
  - `r` (Read), `w` (Write), `x` (Execute).
  - Example: `chmod 755 file.txt` (Owner: read/write/execute, Group: read/execute, Others: read/execute).
- **Ownership (`chown`)**:
  - Change file owner: `chown user:group file.txt`
- **Symbolic Links (`ln -s`)**:
  - Create a shortcut/reference to another file.

## Journaling & Logs

- **Journaling**: A feature that keeps track of file system changes before writing them permanently to prevent corruption.
- **Log Files**:
  - `/var/log/syslog` → System logs.
  - `/var/log/dmesg` → Kernel logs.
  - `/var/log/auth.log` → Authentication logs.

## Special Files

- **Device Files (`/dev/`)**:
  - `/dev/sda` → First hard disk.
  - `/dev/null` → Discard anything written to it.
  - `/dev/random` → Generates random data.
