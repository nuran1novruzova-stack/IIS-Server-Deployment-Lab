# Windows Server 2019 Core — IIS Web Server Deployment & Phishing Test Lab

This repository documents the step-by-step deployment of the IIS (Internet Information Services) web server role on a **Windows Server 2019 Core** environment using PowerShell. It also includes hosting a custom HTML/CSS test page simulating a social media login interface for educational and security testing purposes.

---

## 📋 Project Specifications & Stack

- **Operating System:** Windows Server 2019 Core
- **Web Server:** IIS (Internet Information Services)
- **Management & Automation:** Windows PowerShell
- **Virtualization:** Oracle VM VirtualBox
- **Frontend Stack:** HTML5, CSS3
- **Network Mode:** Bridged Adapter

---

## 🛠️ Step-by-Step Implementation

### 1. IIS Role Installation via PowerShell
Enabled the IIS Web Server role along with management tools on Windows Server Core using the following command:
2. Custom Web Page Deployment
Cleared default IIS landing files located at C:\inetpub\wwwroot.

Created a custom index.html file using Notepad containing a simple Instagram login interface mock-up:

HTML
<html>
<body style="background:#fafafa; text-align:center; font-family:sans-serif">
    <div style="background: white; border: 1px solid #dbdbdb; margin:50px auto; padding:40px; width:300px">
        <h1 style="font-style: italic">Instagram</h1>
        <input type="text" placeholder="Username"><br><br>
        <input type="password" placeholder="Password"><br><br>
        <button style="background:#0095f6; color:white; border: none; padding:7px 20px; border-radius:4px">Log in</button>
    </div>
</body>
</html>
3. Network Configuration & Verification
Set the VirtualBox network mode to Bridged Adapter to assign the server a valid IP on the local subnet.

Retrieved the server's internal IP address via ipconfig.

Successfully verified access to the hosted web page from the host machine's browser using the server's IP.

🔮 Future Enhancements & Real-World Application
This lab setup represents a baseline structure for web service testing and phishing simulation labs. Potential future improvements include:

Replicating official brand styling, logos, and fonts for realistic Red Team / Social Engineering assessments.

Integrating a backend database (SQL Server / MySQL) to handle data inputs and form submissions.

Binding SSL/TLS certificates for HTTPS encryption.

⚠️ Disclaimer
This project was developed strictly for educational, lab testing, and authorized cybersecurity research purposes in an isolated environment. Unethical or unauthorized use of phishing interfaces is illegal.
