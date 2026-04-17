# Modern Cybersecurity Landscape

## Lesson 1: Modern Cybersecurity Landscape

**1.1 The Role of Cybersecurity**
Cybersecurity is a set of practices designed to protect systems, networks, applications, and data from digital attacks, unauthorized access, and disruption. In the modern era, maintaining a robust cybersecurity posture is a corporate responsibility to ensure the safety of user data and business continuity.

**1.1.1 Essential Cybersecurity Terminology**
No system is completely risk-free. However, we can manage risks and reduce the **Attack Surface** (the sum of all points where an attacker can try to enter) by applying **Defense-in-Depth** (layered security).

* **Vulnerability:** A weakness in software, hardware, or processes that can be exploited.
* **Exploit:** A piece of software or a sequence of commands that takes advantage of a vulnerability.
* **Malware:** Malicious software (Viruses, Worms, Trojans) designed to damage or gain unauthorized access.
* **Ransomware:** A type of malware that encrypts files and demands payment for the decryption key.
* **Zero-Day Vulnerability:** A flaw that is unknown to the vendor and has no available patch.
* **Defense-in-Depth:** A security strategy that uses multiple layers of defense so that if one fails, others are in place to stop the threat.

---

**1.2 The Evolving Threat Landscape**
Cyber threats are growing in speed, scale, and sophistication, especially with the integration of AI.

* **Ransomware-as-a-Service (RaaS):** A business model where developers lease ransomware tools to "affiliates," allowing even low-skilled attackers to launch sophisticated campaigns.
* **Supply Chain Attacks:** Indirect attacks that compromise a trusted third-party vendor or software partner to gain access to the main target's network.
* **Credential Theft:** Often achieved through **Phishing**, where attackers steal login info. Since many users reuse passwords, one stolen credential can open multiple doors.
* **AI-Enabled Attacks:** Using AI to automate reconnaissance and create highly convincing phishing messages that are harder to detect than traditional spam.

---

## Cloud Infrastructure Threats

Cloud Security operates under a **Shared Responsibility Model**. While the provider secures the hardware, the customer is responsible for what happens *inside* the cloud (data, identities, and configurations).

**Common Cloud Threats Include:**
* **Misconfigurations:** Leaving storage buckets (like S3) open to the public.
* **Over-privileged Access:** Giving users more permissions than they actually need to do their jobs.
* **Insecure APIs:** Exposed interfaces that allow attackers to bypass standard security.
* **Lack of Visibility:** Not knowing what assets are running in the cloud.

---

**SaaS Application Challenges and Security Risks**
SaaS apps (Slack, Zoom, Salesforce) are essential but introduce unique risks regarding data sharing.

* **Malicious Outsiders:** External actors using SaaS platforms as a delivery vector for malware.
* **Malicious Insiders:** Employees who intentionally leak or steal company data.
* **Data Exposure Risks:**
    * **Accidental Share:** Sending sensitive data to the wrong person by mistake.
    * **Promiscuous Share:** Sharing data with "everyone in the organization" or "anyone with the link," making it accessible to too many people.
    * **Ghost Share:** When access remains active for an ex-employee or a vendor who no longer works with the company.

---

## Lesson 2: Attacker Profiles and Cyberattack Lifecycle

**Attacker Profiles**
* **Cybercriminals:** Motivated primarily by financial gain (the most common profile).
* **Hacktivists:** Attackers motivated by political, social, or religious causes.
* **State-Sponsored Actors (APTs):** Highly sophisticated groups funded by governments for espionage or sabotage.
* **Insiders:** Employees or contractors who have legitimate access but use it maliciously (or accidentally cause harm).
* **Script Kiddies:** Inexperienced attackers who use pre-made tools and scripts found online.

**The Cyberattack Lifecycle (Kill Chain)**
To stop an attack, we must understand its stages:
1.  **Reconnaissance:** Researching the target and looking for vulnerabilities.
2.  **Weaponization:** Creating a malicious payload (e.g., an infected PDF).
3.  **Delivery:** Sending the payload to the target (via email, USB, or web).
4.  **Exploitation:** The malicious code runs and triggers the vulnerability.
5.  **Installation:** The attacker gains a "foothold" (backdoor) in the system.
6.  **Command and Control (C2):** The attacker takes remote control of the compromised system.
7.  **Actions on Objectives:** Stealing data, encrypting files, or disrupting services.

---

## Zero Trust Model
The **Zero Trust** model is a strategic approach to cybersecurity that eliminates the concept of "implicit trust." It doesn't matter if you are inside or outside the office network; everyone must be verified.

**The Three Pillars of Zero Trust:**
1.  **Verify Explicitly:** Always authenticate and authorize based on all available data points (identity, location, device health).
2.  **Least Privilege Access:** Give users access only to the resources they need for that specific moment—nothing more.
3.  **Assume Breach:** Operate as if an attacker is already inside the network. This involves segmenting the network and monitoring all activity to minimize the "blast radius" of an attack.