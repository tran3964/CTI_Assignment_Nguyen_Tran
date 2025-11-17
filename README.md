CTI Assignment
-----------------------------------

## Diamond Model Analysis

This section presents a structured overview of the Diamond Model components based on the selected threat report.

### Components:

### **Adversary – Who is behind the attack**
- Two primary roles exist:  
  **Operator** (the one who executes the attack) and **Customer** (the one who benefits from it).  
- Both the operator and customer can be the same person or organization.  
- In complex or multi-layered cybercrime operations, these roles are intentionally separated to avoid being tracked.  
- High-profile cyberattacks often involve multiple operational teams such as:  
  - Initial access operators  
  - Malware developers  
  - Data exfiltration teams  
- Because of this complex structure, it is extremely difficult to identify the actual operator.  
  Attackers may outsource access, license malware from third parties, and rely on affiliates to deploy attacks.  
  Therefore, investigators can usually only trace the **Adversary customer**, not the operator.

---

### **Capability – How the attack was performed**
- Refers to the **tactics, techniques, and procedures (TTPs)** used by the adversary.  
- Two major categories:  
  - **Tools:** Hacking tools, malware, exploits used during the attack  
  - **Tradecraft:** The attacker’s behavior, methods, and techniques  
- Tools and tradecraft are usually customized for each operation, meaning general tools are less useful for attribution.  
- Characteristics that uniquely identify an adversary include:  
  - Specific malware configuration choices  
  - Custom-developed malware  
  - Novel attack techniques or command-line patterns  
- These key indicators help analysts track and differentiate attack campaigns, aligning findings with phases of the **Cyber Kill Chain**.

---

### **Infrastructure – What resources were used**
Common types of infrastructure include:
- Service accounts  
- Email addresses  
- IP addresses  
- Domains  
- C2 servers  
- Personas (social media handles, phone numbers, Telegram channels, etc.)  
- Cloud services  
- File-sharing websites  
- Tor nodes  
- Compromised websites  

Each operation prioritizes certain infrastructure types depending on the attacker’s strategy, often combining multiple methods for support.

---

### **Victim – Who was targeted**
- The Victim is the entity impacted by the attack or the recipient of the adversary’s Capabilities deployed across their Infrastructure.  
- Victims can be individuals or organizations whose systems, networks, or data are affected.  
- Adversaries typically target victims for their assets, not their identity.  
- Correctly identifying the true victim is important — e.g., a supply chain attack may compromise a vendor to reach a different final target.

---

## Example - Task 3: Extract Diamond Model Elements
**Research Website:**  
https://cloud.google.com/blog/topics/threat-intelligence/vietnamese-actors-fake-job-posting-campaigns  

**Title:**  
*Help Wanted: Vietnamese Actors Using Fake Job Posting Campaigns to Deliver Malware and Steal Credentials*

---

## Diamond Model Table (Based on Selected Report)

| Component | Findings |
|----------|----------|
| **Adversary** | Threat actors targeting Vietnam’s digital job market, exploiting economic pressures and tricking job seekers with fake recruitment campaigns. |
| **Infrastructure** | Websites, Gmail accounts, URLs, messaging platforms used to deliver malicious files or communicate with victims. |
| **Capability** | Malware embedded in PDF files, ZIP archives, or delivered through phishing links. |
| **Victim** | Job seekers, remote workers, and tech professionals applying for online positions. |
