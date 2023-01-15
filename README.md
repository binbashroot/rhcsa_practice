# Practice Exam for RHCSA

### Perform the following tasks

**Any files in a user's home directory must be owner/group of the user**

### Task 1
**Add the following repos to the system**
> BaseOS 
>> http://servera.example.com/repo/BaseOS  

> AppStream  
>> http://servera.example.com/repo/AppStream  

### Task 2
**Install a web server**
> Install the httpd package
> The web services must survive a reboot
> Validate your installation using a web browser @ http:://192.168.1.150/repo


### Task 3
**Add a new partition** 
> Create a 850M partition on your primary disk  
> Create and mount an ext3 filesystem on /mnt/task3  
> The mount point must survive a reboot

### Task 4
**Create a script**
> The script is called task4.sh
> The script must create five files in /opt/dc  
> The filenames are superman, batman, aquaman, flash, wonderwoman  
> The script must reside in /opt/scripts
> The file name extension must be ".out"
> Each file must contain the current date and time
> The script must only be executable by root

### Task 5
**Create a script**
>- [ ] The script is named task5.sh 
>- [ ] The script must reside in /opt/scripts
>- [ ] The script must create five users  
>- [ ] All users must be part of the goodguys group  
>- [ ] The script should only be executable by root
>- [ ] All users must belong to the group named "marvel"
>> spiderman  
>> wolverine  
>> thor  
>> hulk  
>> ironman  

### Task 6
**Create a script**
>- [ ] The script is named task6.sh  
>- [ ] The script must reside in /opt/scripts  
>- [ ] The script must create five users  
>- [ ] All users must be part of the badguys group  
>- [ ] The script should only be executable by root
>- [ ] All users must belong to a secondary group named "marvel"
        sandman
        sabertooth
        loki
        thanos
        ultron

### Task 7
**Create a text file**
>- [ ] The file must reside in /home/student  
>- [ ] The file must be called task7.txt  
>- [ ]  The file must contain the partition table of the primary disk

### Task 8
**Create a text file**
>- [ ] The file must reside in /home/student
>- [ ]  The file must be called second_disk.txt

### Task 9
**Create a text file**  
***NOTE:***  
You will run the following command as your starting point:  
***getent group marvel|cut -d: -f4|tr , '\n'***   

- [ ] File must be called marvel_tb_3.txt
- [ ] File must contain the top and bottom three users of the full sorted list

### Task 10
Create a file in /home/student
        File must be created using stdin/stdout redirect
        File must be called marvel_top3.txt
        File must only have the top 3 alphabetically sorted users
        Using shell commands, get the 3 top and bottom lines from t

### Task 11
Add a new partition to your primary disk
        1 650M partition

### Task 12
Create a directory called /opt/heros
        The owner of the folder should be root
        The group of the folder should be goodguys 
        The permissions of the folder should only allow root and users in the goodguys group access to read/write files, but everyone should be able "list" files

### Task 13
Create a directory in /opt called villians 
        The owner of the folder should be root
        The group of the folder should be villians
        The permissions of the folder should only allow root and users in the badguys group access to read/write files.  root user and users must be able to list files but all other users should not be able to list the contents of the /opt/villians directory

### Task 14
Add a three new partitions to your secondary disk
        One partition must be 500MiB in size
        One partition must be 250MiB in size
        The partition that is 250MiB should have an ext3 filesystem
        The partition that is 100MiB should have an xfs filesystem
        The ext3 filesystem should be mounted on /opt/ext3
        The xfs filesystem should be mounted on /opt/xfs

### Task 15
1. Copy all the files in the /opt/test1 dirs to a directory called /opt/copied
1. The mode for /opt/copied should be  
    1. owner read/write/execute  
    1. group   read/execute  
    1. other   read/execute  

1. File permissions for all files in /opt/copied should be  
    1. owner = student 
    1. group = goodguys

1. files should be readable by the world
1. Files should be read and writeable by the owner 
1. files should be readable and writable by the group 


### Task 16
1. Create the /opt/moved directory if it does not exist
    1. /opt/moved should be owned by student
    1. /opt/moved should belong to the student group
    1. Move all the files in /opt/test2 to /opt/moved
    1. confirm permissions of all files inside /opt/moved
    1. Permissions of all files should be owned by student
    1. Permissions of all files owned by the student group
    1. Files should be read and writeable for user and read-only for group and world
    1. All users on the system should be able to list all files in the /opt/moved directory

### Task 17
/opt/test3 task
1.Create a compressed tarfile called test3.targz of all the files from /opt/test3 
2.Place the compressed file in /tmp
3.The file must use gzip compression





### Bonus tasks
1. change the hostname to andy.example.com and ensure it persists on reboot
1. Change the network interface to 192.168.1.149
1. find and copy all files owned by "albert" into /tmp
