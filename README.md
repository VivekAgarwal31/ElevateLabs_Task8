# 🛡️ VPN Setup and Privacy Analysis – Task 8  
**By:** Vivek Agrawal  
**Date:** November 1, 2025  
**Environment:** Kali Linux and Windows  

---

## 🎯 Objective
The objective of this task was to **set up a Virtual Private Network (VPN)**, analyze how it protects user privacy and network traffic, and validate the difference in IP visibility and data security before and after connection.  
This exercise focuses on understanding **encryption, tunneling, and anonymity** in VPN technology.

---

## 🧰 Tools and Resources
- **ProtonVPN (Free & Open-Source Client)** – for VPN connection and encryption testing  
- **Wireshark** – for capturing and analyzing packet traffic  
- **IP Leak Test Tools** – `https://ipleak.net` and `https://dnsleaktest.com`  
- **Kali Linux Terminal / PowerShell** – to perform traceroute and IP verification  

---

## ⚙️ Methodology
1. Installed and configured **ProtonVPN** on Kali Linux and Windows.  
2. Logged in and connected to multiple VPN servers located in **Singapore**, **United States**, and **Netherlands**.  
3. Verified the **public IP address** before and after VPN activation.  
4. Used **Wireshark** to capture traffic for both states:
   - Before VPN connection (unencrypted traffic)
   - After VPN connection (encrypted/tunneled packets)
5. Conducted **DNS and IP leak tests** using online tools.  
6. Compared the packet encryption and routing paths (via `traceroute` or `tracert`).  
7. Documented results and created screenshots for validation.

---

## 🌐 Observations

| Parameter | Before VPN | After VPN | Remarks |
|------------|-------------|------------|----------|
| **IP Address** | Displayed actual local ISP address | Masked by VPN server IP | VPN successfully hides real IP |
| **DNS Requests** | Routed through local ISP DNS | Routed through VPN DNS servers | Prevents DNS leaks |
| **Packet Encryption** | Plain and readable traffic | Encrypted via OpenVPN tunnel | Traffic confidentiality ensured |
| **Traceroute** | Shows direct ISP path | Routes through VPN nodes | Location obfuscation successful |
| **Latency** | 10–25 ms | 70–120 ms | Slightly increased due to encryption overhead |

---

## 📊 Findings
- VPN effectively **encrypts data packets**, ensuring confidentiality and integrity.  
- The **public IP address** is completely masked, preventing tracking by websites or ISPs.  
- **DNS leak protection** and **kill switch** features were validated in ProtonVPN.  
- Slight increase in latency observed due to encryption and routing.  
- Network activity on Wireshark confirmed **AES-256 encrypted packets**.  

---

## 🧠 Learnings and Insights
- VPNs operate through **secure tunneling protocols** like OpenVPN, WireGuard, and IKEv2.  
- They provide **data confidentiality, location masking, and protection against eavesdropping**.  
- Free VPNs may have **limited bandwidth or logging risks**, so verified providers are preferred.  
- VPNs do **not guarantee anonymity** if users log in to accounts or use identifiable information.  
- Periodic privacy checks like **DNS leak tests** are essential for security validation.  

---

## 💡 Best Practices for VPN Usage
1. Use VPNs that have **no-log policies** and **independent audits**.  
2. Always enable **Kill Switch** and **Auto-Connect** features.  
3. Avoid connecting through **public or free Wi-Fi** without VPN protection.  
4. Combine VPN with **browser privacy extensions** (uBlock Origin, HTTPS Everywhere).  
5. Test your VPN regularly using **IP leak** and **DNS leak** verification tools.  
6. Disconnect VPN only after closing all network-dependent applications.  

---

## 📁 Deliverables
- `VPN_Setup_Report.pdf` — Detailed analysis and screenshots.  
- `README.md` — Summarized documentation of process and findings.  
- `Screenshots/` — Evidence of Analysis.  

---

## 🏁 Conclusion
The VPN setup and privacy analysis demonstrated how encryption and tunneling safeguard network traffic and user identity.  
By routing data through secure tunnels and masking the original IP, VPNs enhance **anonymity, security, and confidentiality** in online communications.  
This task successfully reinforced practical knowledge of **network encryption, packet analysis, and data privacy fundamentals**.

---

> ✨ *Prepared by Vivek Agrawal as part of the Cybersecurity Internship — Task 8 (VPN Setup and Privacy Analysis), November 2025.*
