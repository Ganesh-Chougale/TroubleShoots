### **1️⃣ Enable Clipboard & Drag-Drop (For All OSes)**
1. Open **VirtualBox Manager**  
2. Select your VM → **Settings** → **General** → **Advanced**  
3. Set:  
   - **Shared Clipboard** → **Bidirectional**  
   - **Drag’n’Drop** → **Bidirectional**  
4. Click **OK**, then **start your VM**  

---

### **2️⃣ Install VirtualBox Guest Additions (Required for Full Clipboard Support)**  

#### **📌 Windows Guest VM**  
- Start Windows VM → In **VirtualBox menu**, go to:  
  **Devices → Insert Guest Additions CD Image**  
- Open **File Explorer** → Run `VBoxWindowsAdditions.exe` → Install & Restart  

#### **📌 Linux Guest VM (Ubuntu, Debian, RHEL, CentOS, etc.)**  
1. Open terminal, install dependencies:  
   ```sh
   sudo dnf install epel-release -y  # For RHEL/CentOS  
   sudo dnf install kernel-devel kernel-headers gcc make perl -y
   sudo apt update && sudo apt install build-essential dkms -y  # For Debian/Ubuntu  
   ```
2. In VirtualBox, go to **Devices → Insert Guest Additions CD Image**  
3. Run these commands:  
   ```sh
   sudo mount /dev/cdrom /mnt
   sudo /mnt/VBoxLinuxAdditions.run
   reboot
   ```
4. **After reboot, clipboard sharing should work!**  

#### **📌 macOS Guest VM**  
- VirtualBox **does not fully support macOS Guests** (clipboard might not work).  
- Try enabling clipboard in **Settings → General → Advanced**.  
- For better macOS support, use **VMware or Parallels Desktop**.  

---

### **3️⃣ Test Clipboard Sharing**
✅ Copy-paste text **between host & VM**  
✅ Try **drag-and-drop** between host & VM  
