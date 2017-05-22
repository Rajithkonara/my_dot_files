#Use To remove duplicate lines


The du –sch /path/to/directory/* command returns the disk space usage per subdirectories and files within the specified directory in human-readable format 
(also shows a total per directory) and does not order the output by size:nohlsearch
but by subdirectory and file name.


$ du -sch /var/* | sort -h 
