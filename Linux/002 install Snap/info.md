1. **Update your system:**
   Before proceeding, make sure your system is up-to-date.

   ```bash
   sudo apt update
   sudo apt upgrade
   ```

2. **Install Snapd:**
   To install Snap on Ubuntu 14.04, you need to install `snapd` (Snap Daemon).

   ```bash
   sudo apt install snapd
   ```

3. **Enable Snapd service:**
   After installation, make sure `snapd` is running:

   ```bash
   sudo systemctl enable snapd
   sudo systemctl start snapd
   ```

4. **Check Snap installation:**
   Verify that Snap is installed and working correctly:

   ```bash
   snap version
   ```