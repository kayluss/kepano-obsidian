---
created: 2026-02-01T08:13:00
tags:
  - note
  - journal
---
**Using `ifuse` and `libimobiledevice-utils`**:

- Install the necessary packages:
    
    ```
    sudo dnf install ifuse libimobiledevice-utils  # Fedora
    sudo apt install ifuse libimobiledevice-utils  # Ubuntu/Debian
    ```
    
- Unlock your iPad and pair it with your Linux machine:
    
    ```
    idevicepair pair
    ```
    
- Create a mount point and mount the iPad:
    
    ```
    sudo install -d /mnt/ipad -o $USER
    ifuse /mnt/ipad
    ```
    
- Access files via `/mnt/ipad/`. Use `ls -alh /mnt/ipad/` to list contents.
    
- Always unmount after use: `umount /mnt/ipad`.