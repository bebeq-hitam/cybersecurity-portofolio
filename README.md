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

    > *[Insert Screenshot of Metasploit success here if available]*

3.  **Mitigation & Recovery Strategy**
    * **Immediate Action:** Patch the OS with Microsoft Security Bulletin MS17-010.
    * **Long-term:** Migrate legacy Windows 7 systems to supported OS (Windows 10/11 or Linux).
    * **Compliance:** Prepare the infrastructure for **ISO27001** certification to ensure standard security controls are in place.

---

* **Technical Arsenal:**
  * **Offensive:** Metasploit, Cobalt Strike (Study), Burp Suite.
  * **Development:** C++ , Python , Bash.
  * **Soft Skills:** Strategic Planning (TSA Language Div. Head), Negotiation & Public Speaking.

* **Contact:** [ezar.dega17@gmail.com](mailto:ezar.dega17@gmail.com) | [https://www.linkedin.com/in/ezar-dega-auffa-36582a328/]

---
