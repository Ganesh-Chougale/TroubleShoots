### ✅ **Step 1: Uninstall Node.js from Control Panel**  
1. **Open Control Panel** → Go to **Programs & Features**  
2. Find **Node.js** → Right-click → **Uninstall**  
3. Restart your PC after uninstallation.  

---

### ✅ **Step 2: Delete Leftover Files**  
Manually remove leftover files in these locations:  

```bash
C:\Program Files\nodejs
C:\Users\YourUsername\AppData\Roaming\npm
C:\Users\YourUsername\AppData\Roaming\npm-cache
C:\Users\YourUsername\.npmrc
C:\Users\YourUsername\.node-gyp
C:\Users\YourUsername\AppData\Local\npm
C:\Users\YourUsername\AppData\Local\npm-cache
```
**To delete them quickly:**  
1. **Press `Win + R`**, type `%appdata%`, and press **Enter**  
2. Go to **npm & npm-cache** folders → Delete them  
3. **Press `Win + R`**, type `%localappdata%`, and press **Enter**  
4. Delete **npm** and **npm-cache** folders.  

---

### ✅ **Step 3: Remove from Environment Variables**  
1. **Press `Win + R`**, type `sysdm.cpl`, and press **Enter**  
2. Go to **Advanced** → Click **Environment Variables**  
3. Find **PATH** under **System Variables** → Click **Edit**  
4. Remove any entry related to **Node.js** (`C:\Program Files\nodejs`)  
5. Click **OK** → Restart your PC.  

---

### ✅ **Step 4: Verify Node.js is Removed**  
Open **Command Prompt (cmd)** and run:  
```bash
node -v
npm -v
where node
```
If Node.js is completely removed, these commands should return **"not found" or not recognized.**  

---

### 🔄 **Step 5: Reinstall Node.js (Latest Version)**  
1. **Download Node.js LTS** from [official website](https://nodejs.org)  
2. Run the installer **(Choose LTS version for stability)**  
3. Select **Add to PATH** during installation  
4. Finish and restart your PC.  

---

### ✅ **Step 6: Verify Installation**  
Run in **Command Prompt:**  
```bash
node -v  # Should print latest Node.js version
npm -v   # Should print latest npm version
```

---

### 🚀 **Done! Your Node.js is Clean & Fresh!**  
Now, reinstall your project dependencies:  
```bash
cd your-project
npm install
npm start
```