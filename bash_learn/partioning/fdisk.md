## Reference (http://www.tecmint.com/create-partitions-and-filesystems-in-linux/ )

## Managing MBR Partitions with fdisk

## operations
```sh
$ fdisk /dev/sdb
```
## Managing GPT Partitions with gdisk 
```sh
$ gdisk /dev/sdb
```
## creating file systems
```sh
mkfs -t [filesystem] -L [label] device
```
 or
```sh
mkfs.[filesystem] -L [label] device
```
## Creatign and using Swap Partitions

we need to add the following entry to the /etc/fstab file (X can be either b or c)
```sh
$ /dev/sdX1 swap swap sw 0 0 
```
## Format and enable
```sh
$ mkswap /dev/sdX1
$ swapon -v /dev/sdX1
```
## Display Swap partitions
```sh
$ swapoff /dev/sdX1
```








