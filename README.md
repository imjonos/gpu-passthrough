# Gpu passthrough
GPU Passthrough (Qemu) Intel + Nvidia + Prime

# Installation 

1) sudo apt install qemu-kvm libvirt-bin ubuntu-vm-builder bridge-utils virt-manager (https://help.ubuntu.ru/wiki/kvm)

2)  /etc/default/grub (https://wiki.debian.org/VGAPassthrough)

Add intel_iommu=on on the kernel commandline

GRUB_CMDLINE_LINUX_DEFAULT="intel_iommu=on"

run update-grub 

reboot

3) sudo apt install nvidia-prime (https://help.ubuntu.ru/wiki/nvidia-prime)

4) Create VM (example qemu.xml)

# Using

Run intel

After reboot run w10start
