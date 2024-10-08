# How to Enable Only IPv4 or IPv6 in Windows

This guide will show you how to turn on or off IPv4 or IPv6 on your Windows computer.

## Steps to Follow:

### 1. Open Control Panel
- Press `Win + R` on your keyboard.
- Type `control` and hit **Enter**.

### 2. Go to Network Settings
- Click on **Network and Internet**.
- Then click on **Network and Sharing Center**.
- On the left side, click **Change adapter settings**.

### 3. Open Adapter Properties
- Find your active network (like Ethernet or Wi-Fi).
- Right-click on it and select **Properties**.

### 4. Turn On or Off IPv4 or IPv6
- In the window that pops up:
  - To turn off IPv4, uncheck **Internet Protocol Version 4 (TCP/IPv4)**.
  - To turn off IPv6, uncheck **Internet Protocol Version 6 (TCP/IPv6)**.
- Click **OK** to save your changes.

## Troubleshooting:
- **If you lose internet after turning off IPv6:** Just turn it back on and restart your computer.
- **If you lose internet after turning off IPv4:** Make sure your internet provider supports IPv6 or turn IPv4 back on.

## Reset Network Settings (If Needed)
If things go wrong, you can reset your network settings:
1. Open **Command Prompt** as an Admin (right-click and choose **Run as administrator**).
2. Type these commands one at a time, pressing **Enter** after each:
   ```
   netsh int ip reset
   ipconfig /release
   ipconfig /renew
   ```

### Remember:
If you need both IPv4 and IPv6, go back and make sure both are checked in the Properties window!
