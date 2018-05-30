#### Run dolphin as root in Plasma desktop

Tested on Fedora KDE 27/28 64bit
Tested on Ubuntu KDE 18 64bit
#### How to install
*Note: After system updates (where dolphin/kate have been updated) binaries are need to be replaced again.*

Find preinstalled binaries location:
```bash
find / -name "./libkdeinit5_dolphin.so"
```
Overwrite preinstalled Dolphin binaries
```bash
cp ./libkdeinit5_dolphin.so /usr/lib64/ #Fedora
cp ./libkdeinit5_dolphin.so /usr/lib/x86_64-linux-gnu/ #Kubuntu
```

Overwrite Kate binary
```bash
cp ./kate /usr/bin/
```
