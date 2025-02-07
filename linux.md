# Basic Linux

<kbd>![image](img/linux.png)</kbd>

## General Linux Concepts

- **Linux Kernel**: The core part of the Linux operating system that manages hardware and system resources.
- **Shell**: A command-line interface that allows users to interact with the operating system. Examples: Bash, Zsh, Fish.
- **Terminal**: A program that provides access to the shell (e.g., GNOME Terminal, Konsole, xTerm).

## File System & Navigation

- **Root (`/`)**: The top-level directory of the Linux filesystem.
- **Home Directory (`/home/username`)**: The personal directory for a user.
- **Path**: The location of a file or directory in the filesystem.
  - **Absolute Path**: Full path starting from `/` (e.g., `/home/user/documents`).
  - **Relative Path**: Path relative to the current directory (e.g., `./documents`).
- **Hidden Files**: Files that start with a dot (`.`), like `.bashrc`.
- **Symbolic Link (`ln -s`)**: A shortcut or reference to another file or directory.

## Common Linux Commands

- **Navigation & File Management**:

  - `ls` → List files and directories.
  - `cd` → Change directory.
  - `pwd` → Show current directory.
  - `mkdir` → Create a new directory.
  - `rm` → Remove files or directories.
  - `cp` → Copy files or directories.
  - `mv` → Move or rename files.
  - `find` → Search for files in a directory.

- **File Viewing & Editing**:

  - `cat` → Display file contents.
  - `less` / `more` → View file contents one page at a time.
  - `nano`, `vim`, `emacs` → Text editors in Linux.

- **User & Permissions**:

  - `whoami` → Show the current logged-in user.
  - `id` → Display user ID and group ID.
  - `chmod` → Change file permissions.
  - `chown` → Change file ownership.
  - `sudo` → Execute commands as a superuser (root).

- **Process Management**:

  - `ps` → Show running processes.
  - `top` / `htop` → Display system resource usage.
  - `kill` → Terminate a process.
  - `bg` / `fg` → Manage background and foreground processes.

- **Networking**:

  - `ping` → Test network connectivity.
  - `curl` / `wget` → Download files from the internet.
  - `netstat` / `ss` → Display network connections.
  - `ip` / `ifconfig` → Show IP address and network configuration.

- **Package Management**:
  - **Debian-based (Ubuntu, Debian)**:
    - `apt-get` / `apt` → Install, update, and remove packages.
  - **RedHat-based (RHEL, CentOS, Fedora)**:
    - `yum` / `dnf` → Install, update, and remove packages.
  - **Arch-based (Arch, Manjaro)**:
    - `pacman` → Manage packages.
  - **Snap & Flatpak** → Universal package management systems.

## System Administration

- **Cron Jobs (`crontab`)**: Scheduled tasks in Linux.
- **Logs (`/var/log/`)**: System and application logs.
- **Services (`systemctl` / `service`)**: Manage system services.
- **Disk Usage & Monitoring**:
  - `df` → Show disk space usage.
  - `du` → Show directory size.
  - `free` → Display memory usage.

## Linux Distributions

- **Debian-based**: Ubuntu, Debian, Linux Mint.
- **RedHat-based**: RHEL, CentOS, Fedora.
- **Arch-based**: Arch Linux, Manjaro.
- **Other popular distros**: OpenSUSE, Alpine, Kali Linux.

## Special Characters in Linux

- `.` → Current directory.
- `..` → Parent directory.
- `~` → Home directory.
- `*` → Wildcard (matches multiple files).
- `|` → Pipe (pass output from one command to another).
- `>` / `>>` → Redirect output to a file.
- `&` → Run a command in the background.
- `$` → Indicates a shell variable.
