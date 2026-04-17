# Cloud Security Fundamentals

## Cloud Computing Models

**Introduction**
In this section, I explored the different cloud deployment models—Public, Private, and Hybrid—and the various service categories available.

**What Is Cloud Computing?**
Cloud computing is not a specific location, but rather a model for enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable computing resources (e.g., networks, servers, storage, applications, and services) that can be rapidly provisioned with minimal management effort.

**The Benefits of Cloud Computing**
Transitioning to the cloud offers several strategic advantages:
* **Scalability:** Ability to scale resources up or down based on demand.
* **Reduced Expenses:** Shifts costs from Capital Expenditure (CapEx) to Operational Expenditure (OpEx).
* **Segmented Administration:** Granular control over different environments.
* **User-ID Integration:** The ability to share IP-address-to-username mappings across virtual systems to leverage full User-ID visibility and security.

---

### 1. IaaS (Infrastructure as a Service)
**The Foundation.** Here, the cloud provider delivers "raw" hardware resources in a virtualized format. You receive the server, storage, and networking, but you are responsible for installing the Operating System (Linux/Windows), databases, and applications.
* **You manage:** Operating systems, applications, data, and internal network security.
* **Cloud provider manages:** Physical servers, hard drives, power, and the virtualization layer.
* **Examples:** AWS EC2, Microsoft Azure VMs, Google Compute Engine.

### 2. PaaS (Platform as a Service)
**The Developer’s Choice.** The focus is on software development. Instead of managing servers or OS updates, you focus entirely on your code. The provider delivers a ready-to-use platform with the OS and development tools pre-configured.
* **You manage:** Application code and data.
* **Cloud provider manages:** Everything else (OS, security patches, middleware, and server scaling).
* **Examples:** Google App Engine, AWS Elastic Beanstalk, Heroku.

### 3. SaaS (Software as a Service)
**The Highest Level.** This is the most common model for end-users. The software is ready and runs in the cloud. You don't install anything on a server; you simply access it via a web browser or app.
* **You manage:** Basic user settings and access permissions.
* **Cloud provider manages:** Absolutely everything (infrastructure, code, security, and maintenance).
* **Examples:** Microsoft Teams, Outlook, Slack, Salesforce, Netflix.

---

## Cloud Native Technologies

**Introduction**
Cloud-native technologies refer to computing resources deployed via Virtual Machines (VMs), Containers, and Serverless platforms.

### Hypervisors
1. **Type 1 Hypervisor: Bare-Metal**
   Runs directly on the server's physical hardware without a host operating system. It acts as the OS itself, focused exclusively on managing VM resources.
   * **Advantage:** High performance and stability.
   * **Examples:** VMware ESXi, Microsoft Hyper-V, Xen.
2. **Type 2 Hypervisor: Hosted**
   Runs as an application inside a conventional operating system (Windows, Mac, or Linux).
   * **Advantage:** Easy to install; ideal for testing and development.
   * **Examples:** Oracle VirtualBox, VMware Workstation.
3. **KVM (Kernel-based Virtual Machine)**
   The standard for Linux-based cloud infrastructure. It effectively turns the Linux Kernel into a Type 1 Hypervisor. It is highly efficient for running Docker containers and large-scale Linux instances.

---

## Cloud Native Security

### Transport Layer Security (TLS)
TLS is the primary protocol for securing data privacy and communication over the internet. Its core functions include:
* **Encryption:** Hides the data being transferred from third parties.
* **Authentication:** Ensures that the parties exchanging information are who they claim to be.
* **Integrity:** Verifies that the data has not been forged or tampered with during transit.
* **Handshake Protocol:** Securely negotiates the encryption algorithm and keys before data transfer begins.

## Prisma Cloud (CNAPP Solution)
Prisma Cloud secures applications from code to cloud, enabling security and DevOps teams to collaborate effectively to accelerate secure cloud-native application development and deployment. Key features include:
* **Shift-Left Security:** Identifying vulnerabilities early in the development lifecycle (CI/CD).
* **Full-Stack Visibility:** Monitoring the entire environment, from hosts and containers to serverless functions.
* **Threat Detection:** Using machine learning to detect anomalous behavior and potential breaches in real-time.

## Visibility, Compliance, and Governance
Prisma Cloud is a native security platform that provides visibility, compliance, and governance for your public cloud accounts in the face of security threats:
* **IaC (Infrastructure as Code) Scanning:** Automatically checking Terraform, CloudFormation, or Ansible templates for security misconfigurations before deployment.
* **CSPM (Cloud Security Posture Management):** Continuous monitoring to ensure the cloud environment follows compliance standards (like CIS, GDPR, or HIPAA).
* **CWPP (Cloud Workload Protection Platform):** Specialized protection for the "workloads" (the actual running applications) regardless of where they are hosted.
* **CIEM (Cloud Infrastructure Entitlement Management):** Managing identities and ensuring "Least Privilege" access to prevent credential misuse.