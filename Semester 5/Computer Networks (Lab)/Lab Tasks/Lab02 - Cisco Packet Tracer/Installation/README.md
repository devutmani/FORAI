# Cisco Packet Tracer – Installation & Login Bypass Guide

This guide explains how to install Cisco Packet Tracer (using the included setup wizard) and how to bypass the login screen using a firewall rule.

---

## 1. Installation

1. Locate the `CiscoPacketTracer822_64bit_setup_signed.zip` file provided in this directory.  
2. Extract the zip file.  
3. Run the **setup wizard**.  
4. Follow the wizard steps – it will guide you through the installation automatically.  
5. Once installation is complete, launch **Cisco Packet Tracer**.  

⚠️ **Important:** On first startup, the program requires a **Cisco NetAcad login** to enable full usage (saving, exporting, etc.). Since login is mandatory, we will bypass it using the next step.

---

## 2. Login Bypass (Firewall Method)

The login screen can be bypassed by blocking Packet Tracer’s inbound and outbound internet access. This prevents the app from reaching Cisco’s servers, letting it run in offline mode.

### Windows Firewall Steps
1. Open **Windows Defender Firewall**.  
2. Click **Advanced Settings** on the left.  
3. In the **Outbound Rules** section:
   - Click **New Rule…**  
   - Select **Program** → click **Next**.  
   - Browse to `C:\Program Files\Cisco Packet Tracer\bin\PacketTracer.exe`.  
   - Select **Block the connection** → apply to **Domain, Private, Public**.  
   - Name the rule (e.g., `Packet Tracer Outbound Block`) → Finish.  
4. Repeat the same steps in the **Inbound Rules** section.  
5. Launch **Cisco Packet Tracer** again. The login window will appear but authentication will not complete—allowing you to use and save your work offline.  

---
*Video Guide:* [How to Use Cisco Packet Tracer Without User Login | Bypass Logon Session](https://www.youtube.com/watch?v=7yMXQNtBzA0)

## 3. Summary

- Extract the included installer zip and run the setup wizard.  
- Normally, login is required to use Packet Tracer.  
- By blocking inbound and outbound connections via firewall, the login check is bypassed.  

---

## ⚠️ Disclaimer

This login bypass method is **unofficial** and not endorsed by Cisco. Use it only for educational purposes or where permitted by your institution.
