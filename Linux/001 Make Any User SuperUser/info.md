## 1. make vanila user SU
```bash
su
# password
```   
```bash
usermod -aG sudo raskull
```   
## 2. Edit the sudoers File (Optional - if Necessary)  
```bash
visudo
```  
```bash
raskull ALL=(ALL:ALL) ALL
```  