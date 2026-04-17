# Cloud Security: Core Essentials

## 1. Shared Responsibility Model
The most important rule: **Cloud providers protect the cloud; YOU protect what's inside.**

| Model | You Manage | Cloud Provider Manages |
| :--- | :--- | :--- |
| **IaaS** | OS, Apps, Runtime, Data | Servers, Storage, Networking |
| **PaaS** | Application Code, Data | OS, Runtime, Infrastructure |
| **SaaS** | Users, Access, Data | Everything else |

> **Universal Rule:** Data and Identity (IAM) are **ALWAYS** your responsibility.

---

## 2. Hypervisors (The Engine)
* **Type 1 (Bare-Metal):** Direct on hardware. Fast & Secure. (ESXi, Hyper-V).
* **Type 2 (Hosted):** Runs on top of an OS. Good for labs/dev. (VirtualBox).
* **KVM:** Turns Linux Kernel into a Type 1 hypervisor. The backbone of modern cloud.

---

## 3. The Security "Alphabet Soup"
* **CNAPP (Prisma Cloud):** The full platform (Code to Cloud).
* **CSPM:** Finds **misconfigurations** (e.g., "This bucket is public!").
* **CWPP:** Protects the **workload** (e.g., "Is there malware in this container?").
* **CIEM:** Manages **permissions** (Least Privilege principle).
* **IaC Scanning:** Scans code (Terraform) **before** it builds the infra.

---

## 4. TLS Essentials (Privacy)
Ensures three things for data in transit:
1.  **Encryption:** Confidentiality (No eavesdropping).
2.  **Authentication:** Trust (You are who you say you are).
3.  **Integrity:** No tampering (Data hasn't changed).

---

## 5. Key Cloud Attributes
* **On-demand self-service:** Get resources without human interaction.
* **Elasticity:** Scale up (and down) instantly.
* **Resource Pooling:** Multi-tenancy (sharing hardware safely).