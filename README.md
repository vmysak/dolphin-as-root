Run dolphin as root in Plasma desktop

Tested on Fedora KDE 27/28 64bit
Tested on Ubuntu KDE 18 64bit

#How to install

Find preinstalled binaries location:
find / -name "./libkdeinit5_dolphin.so"

Overwrite preinstalled binaries
cp ./libkdeinit5_dolphin.so /usr/lib64/ #Fedora
cp ./libkdeinit5_dolphin.so /usr/lib/x86_64-linux-gnu/ #Kubuntu

Overwrite Kate binary
cp ./kate /usr/bin/
