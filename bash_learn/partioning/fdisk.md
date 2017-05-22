
# Ref - (http://www.tecmint.com/create-partitions-and-filesystems-in-linux/ )

# Managing MBR Partitions with fdisk

#operations

$ fdisk /dev/sdb

# Managing GPT Partitions with gdisk 

$ gdisk /dev/sdb

# creating file systems

# mkfs -t [filesystem] -L [label] device
or
# mkfs.[filesystem] -L [label] device

#Creatign and using Swap Partitions

we need to add the following entry to the /etc/fstab file (X can be either b or c).

$ /dev/sdX1 swap swap sw 0 0 

# Format and enable

$ mkswap /dev/sdX1
$ swapon -v /dev/sdX1

# Displat Swap partitions

$ swapoff /dev/sdX1









