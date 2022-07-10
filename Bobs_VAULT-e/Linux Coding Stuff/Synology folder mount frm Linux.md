

sudo mount 192.168.1.214:/volume1/Downloads /media/NAS/Downloads

sudo mount 192.168.7.247:/volume1/Bobs_Obsidian /media/robert/NAS/Obsidian

/volume1/Bobs_Obsidian

227 = dell ip
192.168.7.227 is the Dell ip address
sudo mount 192.168.7.227:/volume1/Bobs_Obsidian /media/robert/NAS/Obsidian


192.168.1.214:/volume1/Downloads /media/NAS/Downloads nfs rsize=8192,wsize=8192,timeo=14,intr

add this the  /etc/fstab    - file  (do as root admin)
192.168.7.227:/volume1/Bobs_Obsidian /media/robert/NAS/Obsidian  nfs rsize=8192,wsize=8192,timeo=14,intr


Infos at site
https://saywebsolutions.com/blog/mounting_synology_nas_shared_folder_nfs_ubuntu_16_10

https://kb.synology.com/en-us/DSM/tutorial/How_to_access_files_on_Synology_NAS_within_the_local_network_NFS

https://kb.synology.com/en-us/DSM/help/DSM/AdminCenter/file_share_privilege_nfs?version=7


cannot mount except for root 
cannot change permissions with caja admin access


## trying - chown

to test for ownershp
sudo chown robert /media/robert/NAS
ls -l -d /media/robert/NAS

sudo chown -R robert:robert /media/robert/NAS

fuser -a /media/robert/NAS

showmount -e 192.168.7.247

umount -l /media/robert/NAS

umount -l /media/robert/NAS/Obsidian

umount -f /media/robert/NAS/Obsidian
umount -f /media/robert/NAS
sudo mount -t nfs 192.168.7.247:/volume1/Bobs_Obsidian /media/robert/NAS/Obsidian

sudo mount -t nfs 192.168.7.247:/volume1/Bobs_Obsidian /media/robert/NAS/Obsidian





umount -f /mnt/local



<mark style="background: #FFB86CA6;">this mounted the nas</mark> 
sudo mount 192.168.7.247:/volume1/Bobs_Obsidian /media/robert/NAS/Obsidian

the ip in the nas of the control paner shared folder is 
the ip of the Dell pc

![[Pasted image 20220705161731.png]]



















rsync: chgrp "/xxxxx" failed: Operation not permitted











ooooo