# Cybersecurity & Cloud: Must Remember

## 1. The Attacker's Mindset (The Kill Chain)
To stop an attack, you must break one of these links:
1. **Recon:** Researching the target.
2. **Weaponization:** Prepping the malware.
3. **Delivery:** Sending it (Phishing/USB).
4. **Exploitation:** The malware "breaks" the system.
5. **Installation:** Creating a "backdoor" (foothold).
6. **C2 (Command & Control):** Remote control of the victim.
7. **Objectives:** Stealing data or encrypting (Ransomware).

---

## 2. Zero Trust: The Golden Rule
**"Never Trust, Always Verify."**
* **Assume Breach:** Act as if the hacker is already inside.
* **Least Privilege:** Give the bare minimum access needed. No more "Admin" for everyone.
* **Verify Explicitly:** Identity + Device + Location + Context.

---

## 3. SaaS Sharing Risks (The "Promiscuous" Problem)
* **Promiscuous Share:** Sharing with "Anyone with the link" (Public).
* **Ghost Share:** Access left active for people who left the company (Ex-employees).
* **Accidental Share:** Oops, sent the payroll to the "General" channel.

---

## 4. Modern Threat Vocabulary
* **RaaS (Ransomware-as-a-Service):** Hiring a hacker's software to do the dirty work.
* **Supply Chain Attack:** Attacking a small vendor to get into a big company (Target/SolarWinds style).
* **Attack Surface:** All the "doors and windows" (IPs, APIs, Emails) exposed to the internet.
* **Zero-Day:** A hole in the wall that the owner doesn't know exists yet.

---

## 5. Cloud Protection (Shorthand)
* **CSPM:** Fixes **Mistakes** (Configurations).
* **CWPP:** Protects the **Worker** (The running code/server).
* **CIEM:** Fixes **Permissions** (Who can do what).
* **Shift-Left:** Testing for security **before** the code goes live.

---

## 6. Security Foundation (CIA Triad)
* **Confidentiality:** Keep it secret.
* **Integrity:** Keep it original (no changes).
* **Availability:** Keep it running.