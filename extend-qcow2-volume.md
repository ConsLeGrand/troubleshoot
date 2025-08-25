1- Etendre le volume 
```shell
sudo qemu-img resize /chemin/qcow2/disk.qcow2 +960G
```

2- Étendre la partition sur la vm 
```shell
sudo growpart /dev/vda 1   # si ext4
sudo xfs_growfs /           # si XFS
```
