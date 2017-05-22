#Finding files recursively according to the size

$ find . -maxdepth 3 -type f -size +2M

#find and delete files with user permission 777

$ find /home/user -perm 777 -exec rm '{}' + 
