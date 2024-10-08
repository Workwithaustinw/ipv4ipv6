
---

# How to Enable Only IPv4 or IPv6 in Windows Control Panel

This guide will walk you through enabling or disabling either **IPv4** or **IPv6** protocols on your Windows machine through the Control Panel.

## Table of Contents
1. [Prerequisites](#prerequisites)
2. [Enabling/Disabling IPv4 and IPv6](#enablingdisabling-ipv4-and-ipv6)
    - [Windows 10/11](#windows-1011)
3. [Troubleshooting](#troubleshooting)
4. [Additional Resources](#additional-resources)

---

## Prerequisites

- You must have **administrator privileges** on your system to make these changes.
- This guide is intended for Windows 10/11, but may also work for older versions of Windows.

---

## Enabling/Disabling IPv4 and IPv6

### Windows 10/11

1. **Open the Control Panel**:
   - Press `Win + R` to open the Run dialog.
   - Type `control` and press **Enter** to open the Control Panel.

2. **Navigate to Network Settings**:
   - In the Control Panel, click on **Network and Internet**.
   - Then, click on **Network and Sharing Center**.
   - On the left-hand side, click on **Change adapter settings**.

3. **Access Network Adapter Properties**:
   - In the **Network Connections** window, locate the active network connection (e.g., Ethernet, Wi-Fi).
   - Right-click on the network adapter and select **Properties**.

4. **Enable or Disable IPv4/IPv6**:
   - In the **Networking** tab of the properties window, you will see a list of items that the connection uses.
   - To enable or disable **IPv4**:
     - Find and check/uncheck **Internet Protocol Version 4 (TCP/IPv4)**.
   - To enable or disable **IPv6**:
     - Find and check/uncheck **Internet Protocol Version 6 (TCP/IPv6)**.

5. **Save Changes**:
   - After making your selection, click **OK** to apply the changes.
   - Your network connection may briefly reset after enabling or disabling a protocol.

---

### Visual Steps:

1. **Network Adapter Properties**:
   - ![Network Adapter Properties](https://example.com/network-adapter-properties.png)

2. **Enable/Disable IPv4 and IPv6**:
   - ![Enable/Disable IPv4 IPv6](https://example.com/enable-disable-ipv4-ipv6.png)

---

## Troubleshooting

1. **No Internet Connection After Disabling IPv6**:
   - If disabling IPv6 causes your network to lose connectivity, some services may be dependent on IPv6. Re-enable IPv6 and reboot your system to resolve this.

2. **Network Issues After Disabling IPv4**:
   - Most networks still rely on IPv4. Disabling IPv4 may cause you to lose internet access. Ensure your network and ISP fully support IPv6 before disabling IPv4.

3. **Resetting Network Settings**:
   - If you experience any issues after making changes, you can reset your network settings:
     1. Open a Command Prompt as Administrator.
     2. Run the following commands:

        ```bash
        netsh int ip reset
        ipconfig /release
        ipconfig /renew
        ```

4. **Enable Both IPv4 and IPv6 Again**:
   - If you need both IPv4 and IPv6, follow the steps above and ensure both protocols are checked in the Network Adapter Properties window.

---

## Additional Resources

- [How to Use IPv6 on Windows 10](https://support.microsoft.com/en-us/help/929852)
- [Microsoft IPv6 Documentation](https://docs.microsoft.com/en-us/windows/networking/ipv6/ipv6-portal)

---
