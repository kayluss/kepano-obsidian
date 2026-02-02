---
created: 2026-02-01T22:19:00
tags:
  - note
  - journal
categories:
  - "[[Learning]]"
---
When installing software via the [[command line]] on [[Linux]], *files are distributed across standardized system directories based on their type*, rather than being grouped in a single folder like in Windows. 

**Key directories for installed files:**

- **/usr/bin** or **/bin**: Executable programs for regular users and system commands. 
	- I dont know how to run programs without being in this dir. Is That even a thing? [[Questions]]
    
- **/usr/lib** or **/lib**: Shared libraries and support files. 
    
- **/usr/share**: Non-executable data such as icons, artwork, documentation, and configuration templates. 
    
- **/etc**: System-wide configuration files.
    
- **/usr/local**: Often used for locally compiled or manually installed software (especially command-line tools). 
    
- **~/.local/share** or **~/.config**: User-specific data and configuration files.
    

For packages installed via package managers like `apt` (Debian/Ubuntu), use:

- `dpkg -L <package_name>` to list all files installed by a specific package.
    
- `rpm -ql <package_name>` for RPM-based systems (e.g., Fedora, RHEL). 
    

**Note:** There is no single "installation directory" for a program. Instead, files are split across these locations according to the Linux Filesystem Hierarchy Standard (FHS).

