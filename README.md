# AI-Pre-Apprenticeship-Capstone
# Meet my Career Coach

## 1. Project Overview
My AI Career Coach is designed to help graduating Computer Science students
with getting their careers started.

**Career pathway:** Cybersecurity

**Built with:** Google NotebookLM

## 2. The Problem I'm Solving
What career challenge inspired this assistant?
Entering the cybersecurity job market as a new graduate presents a significant structural challenge. Mid-level job postings for Cloud Security Engineers typically require 2–4 years of direct experience with cloud perimeters, identity governance, and detection engineering, alongside specialized credentials such as the AZ-500.

Why would someone benefit from this tool?
An AI Career Coach gives you tailored, evidence backed guidance instead of generic online advice. It directly compares your resume against real job requirements to pinpoint your exact skill gaps, helps you practice technical interview scenarios, and provides a clear, step by step career roadmap.
## 3. How My AI Career Coach Works
I curated resources including:
- Target Job Description: Cloud Security Engineer (Azure) (detailing requirements in Entra ID, Microsoft Sentinel, KQL, Azure Firewall, NSGs, and Key Vault) 
- Industry & Security Frameworks:NIST Cybersecurity Framework (CSF) 2.0 (NIST CSWP 29)
- Academic & Professional Artifacts: Resume & Statement of Qualifications 

I used NotebookLM to analyze these resources and provide source-grounded career guidance.

## 4. My AI Career Coach in Action

### Example 1: Career Guidance
**My prompt:** What skills am I missing for a cloud security role? Base your answer on my resume and the job description. Separate skills I clearly have, skills I may have but haven't demonstrated, and skills I appear to be missing. Point me to the evidence for each.

**What the AI helped me understand:**
The assistant performed a structured audit comparing my resume against the Azure job posting. It highlighted that while I clearly possess **Identity &amp; Access Management (Entra ID, MFA, Conditional Access)** and **SIEM Operations (Splunk, CrowdStrike Falcon)**, I have critical engineering gaps in **Microsoft Sentinel (KQL)**, **Azure Infrastructure Controls (Azure Firewall, NSGs, Key Vault)**, and **Infrastructure as Code (Terraform/Bicep)**.


<img width="1512" height="982" alt="Screenshot 2026-11-05 at 3 07 31 PM" src="https://github.com/user-attachments/assets/c4260735-5c52-41ad-bcab-3691db2fa052" />


### Example 2: Objective Technical Assessment & Bias Mitigation
**My prompt:** 
You are an objective, bias-mitigated technical assessment engine. Strip all demographic, age, lifestyle, and gender-implicit variables from the following input. Evaluate the candidates strictly on a 1-to-5 matrix matching these parameters: [Certifications], [Incident Triage Speed], and [System Documentation History].

**What I learned:** 
My Notebook LM demonstrated responsible AI diligence by stripping away non-job-related personal characteristics (age, lifestyle, family status) and evaluating candidates strictly on verifiable technical evidence. Once personal noise was filtered out, it correctly identified that neither candidate record contained verified technical metrics, returning an objective "N/A" rather than hallucinating arbitrary numerical scores.

<img width="1512" height="982" alt="Screenshot 2026-11-05 at 3 07 50 PM" src="https://github.com/user-attachments/assets/40468cdb-ae8f-448f-bafa-1b8c20d3c997" />


### Example 3: Enterprise Technical Briefing &amp; Operational Synthesis
**My prompt:** 
Take this unstructured text string filter out the conversational noise and organize the data into an enterprise ready technical briefing document using three structured headers: completed tasks, active bottlenecks, and high priority next actions.

**My next steps:** 
Transform unstructured meeting notes and triage outputs into an executive-ready technical briefing. It categorized operational achievements (SIEM migration, email triage automation), flagged active technical bottlenecks (multi-line DMARC strings, Sentinel KQL lab gaps), and established an actionable priority plan for deployment.


<img width="1512" height="982" alt="Screenshot 2026-11-05 at 3 08 29 PM" src="https://github.com/user-attachments/assets/be1aa981-a6d7-4165-89d8-51fdd4074c54" />


## 5. Testing and Improving My Assistant
**Original prompt:** 
Provide a solution to the email triage problem in Python but intentionally include a subtle syntax bug, an unhandled edge case, or an outdated security protocol.

**Improved prompt:**
Act as a code auditor. Read the output to catch the mistake using your core track knowledge. Next, write a corrective follow-up prompt that fixes the intentionally introduced problem, uses RFC-compliant parsing (\`email.utils.parseaddr()\`) to isolate true sending domains from fake display-name strings, and provides a production-ready solution.

**What changed and why:**
The original prompt produced code with a syntax error (\`msg.is\_multipart()\` corrupted) and a logic flaw that allowed display-name email spoofing. The improved prompt forced the AI to perform a code audit, apply RFC-compliant email header parsing to catch display-name spoofing, and deliver production-ready code.

## 6. Responsible AI
How did I check the AI's output for accuracy,
bias, or misleading information?
All technical recommendations, security controls, and code snippets were cross-referenced against official Microsoft Azure documentation and NIST CSF 2.0 standards. Additionally, multi-turn prompt engineering tests were conducted to identify and eliminate algorithmic bias in candidate screening scenarios.

What information should never be shared
with this assistant?
Private API keys, account passwords, internal corporate network IP addresses, unredacted corporate logs, credit union member financial data, or sensitive personally identifiable information (PII).

## 7. My 30/60/90-Day Career Plan
**30 days:** Complete the CompTIA Security+ exam, set up an Azure student lab tenant with Entra ID and Conditional Access, and configure basic Microsoft Sentinel KQL log ingestion.
**60 days:** Build and publish an Infrastructure as Code (IaC) GitHub repository using Terraform/Bicep for Azure Firewall and NSG perimeters, and complete AZ-500 self-study modules.
**90 days:** Refine 5 STAR-formatted interview stories based on internship accomplishments (Splunk to CrowdStrike query migration, Azure AD controls) and apply for SOC Analyst Tier I and Associate Cloud Security Engineer roles.

## 8. Reflection
1. What was the most useful thing my AI coach did? Synthesizing my actual resume bullet points against official Azure job postings and NIST CSF 2.0 to deliver personalized, evidence-backed skills gap audits and verbal interview scripts.
2. What was one limitation or mistake I discovered? Naive prompt instructions produced Python code prone to display name email spoofing and syntax errors, proving that AI outputs must always be audited by a human with domain knowledge.
3. How could this assistant help someone in a real job? It acts as an interactive, on demand SOC mentor that helps security analysts draft incident response playbooks, automate log triage scripts, and translate complex technical findings into executive briefings.
4. What would I improve in a future version? Integrate custom KQL and Terraform validation scripts directly into the assistant's reference corpus to automatically test and lint cloud infrastructure code.

## 9. Skills Demonstrated
- Prompt engineering
- AI output evaluation
- Research and source curation
- Responsible AI practices
- GitHub documentation
- Career readiness
