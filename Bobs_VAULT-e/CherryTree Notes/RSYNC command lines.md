transferred on Saturday, July 09, 2022 -- at 07:45:52 AM
# RSYNC command lines
  
--1

![[Pasted image 20220709074509.png]]
 

rsync -h --progress --stats -r -tgo -p -l -D --update --delete-after /media/robert/SSD-ntfs/TRANSFER /run/user/1000/gvfs/smb-share:server=mediamax21.local,share=4tb_usb/From_SSD-ntfs-Drive/  
  
edited -  
  
rsync -h --progress --stats -r -tgo -p -l -D --update /media/robert/SSD-ntfs/TRANSFER /run/user/1000/gvfs/smb-share:server=mediamax21.local,share=4tb_usb/From_SSD-ntfs-Drive/  
  
  
--2
  
![[Pasted image 20220709074526.png]]
  
rsync -h --progress --stats -r -tgo -p -l -D --update --delete-after /media/robert/SSD-ntfs/Scripts2b /run/user/1000/gvfs/smb-share:server=mediamax21.local,share=4tb_usb/From_SSD-ntfs-Drive/  
  
edited - (remove delete after)  
rsync -h --progress --stats -r -tgo -p -l -D --update /media/robert/SSD-ntfs/Scripts2b /run/user/1000/gvfs/smb-share:server=mediamax21.local,share=4tb_usb/From_SSD-ntfs-Drive/  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
oooooooooooooooooooooo