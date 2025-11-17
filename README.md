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

## Threat Actor Profile Summary - Task 5

This report, titled *"Help Wanted: Vietnamese Actors Using Fake Job Posting Campaigns to Deliver Malware and Steal Credentials"*, examines a campaign carried out by Vietnamese actors. Threat actors target Vietnam's digital job market. Their main objective is to steal credentials and deliver malware, often disguised as part of a scheduled interview process.

In this environment of high competition and widespread remote work, job seekers, remote workers, and tech professionals become valuable targets. Fake job postings spread globally, reaching victims across multiple regions. Because remote work is convenient and appealing, it attracts many people who are seeking job opportunities and can provide a flexible schedule.

As the technology sector becomes increasingly prominent in the job market, adversaries exploit the weak point by sending emails that attach files like PDFs, ZIPs, or phishing URLs delivered to the target. The malicious software hidden inside these files activates once the victim opens or accesses them, allowing the attackers to infiltrate the victim’s system.

As seen in the Diamond Model analysis, the adversary in this campaign is exploiting the trend of the job market. They operate by impersonating recruiters and taking advantage of the benefits of freely posting on job-search platforms where posting and sharing opportunities is easy and largely unverified. Their infrastructure includes messaging platforms, email accounts, and job posting websites that allow them to reach victims directly. Their capability involves hiding malicious code inside documents or URLs, allowing the malware to bypass basic security checks. Then they use any messaging platform to access the target and send their prepared files or URLs.

## Reflection Questions:

### How does the Diamond Model help in understanding threat actors? 

The Diamond Model helps to analyze the adversary's campaign. It will reduce the time for both sides tracking and operating. The diagram can clearly show the association between components.

### What challenges did you face in identifying each vertex? 

Even though the Diamond Model is convenient and initially identifies for victim can be easy, but identifying the adversary might be wrong if that is a complex cyberattack, and tracking their infrastructure and capability is not easy. Because I believe that adversaries always have their ways to hide their malicious intent by overlapping many types of infrastructure and protective capabilities to cut the trace at any time if someone tries to find them.

### How could this model support proactive defense strategies? 

Technically, this model will support proactive defense strategies because it can determine the affected victims and map out the potential entry points used by the attackers.

