# tuen off windows defeneder permenantly  
### 1. turn of windows defender from settings
`Settings`----->`Virus & threat protection`----->`Manage Setting`  
turn of all options  
### 2. disable windows defender permentaly  
`WIN + R`----->`gpedit.msc`  
`Computer Configuration`----->`Administrative Templates`----->`Windows Components`----->`Microsoft Defender Antivirus`  
find:  
turn off Microsoft Defender Antivirus  
and set it from **Not Configures** to **Enabled**  
Apply & Ok.  