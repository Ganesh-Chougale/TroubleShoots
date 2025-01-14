## 1. make vanila user SU
```bash
su
# password
```   
```bash
usermod -aG sudo <userName>
```   
`usermod`: Command to modify a user account.  
`-a`: Append the user to the specified group(s) without removing them from other groups.  
`-G`: Specifies the group(s) to add the user to.  
`sudo`: The group name you are adding the user to. Members of this group can execute commands with elevated privileges using sudo.  
`username`: The username of the account being modified.  

## 2. Edit the sudoers File (Optional - if Necessary)  
```bash
visudo
```  
```bash
raskull ALL=(ALL:ALL) ALL
```  
`ctrl + O` to save or `Ctrl + X` then say yes for save.  