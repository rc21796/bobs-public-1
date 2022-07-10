
# Lucky Backup Setups



--  
![[Pasted image 20220709071822.png]]  
  
  
--  
![[Pasted image 20220709071835.png]]  
  
  
Rsync command -  
  
rsync -h --progress --stats -r -tgo -p -l -D --update /home/robert /run/user/1000/gvfs/smb-share:server=mediamax21.local,share=4tb_usb/Dell-Home-folder-backup/  
  
  
ooooo