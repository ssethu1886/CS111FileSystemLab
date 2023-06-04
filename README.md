## UID: 605742828

# Hey! I'm Filing Here

A 1 MiB ext2 file system with 2 directories, 1 regular file, and 1 symbolic link.

## Building

Type the command "make".

## Running

To compile, type "./ext2-create." Create a directory to mount the file system to with "mkdir mnt".  Mount the filsystem with the command "sudo mount -o loop test.img mnt." Example outpout of 'ls -ain' with  the mounted file system is: 
total 7
      2 drwxr-xr-x 3   0     0 1024 Jun  2 20:53 .
1094656 drwxr-xr-x 4 1000 1000 4096 Jun  2 20:53 ..
     13 lrw-r--r-- 1 1000 1000   11 Jun  2 20:53 hello -> hello-world
     12 -rw-r--r-- 1 1000 1000   12 Jun  2 20:53 hello-world
     11 drwxr-xr-x 2    0    0 1024 Jun  2 20:53 lost+found

## Cleaning up

Unmount the filesystem with the command "sudo unmount mnt". Remove the mount directory with "rmdir mnt." Clean up all binary files with "make clean."
