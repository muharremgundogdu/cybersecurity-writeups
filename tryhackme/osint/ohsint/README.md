# TryHackMe – OHSINT

## 1️⃣ Overview
This write-up documents my analysis of the **OHSINT** room on TryHackMe.  
The objective was to identify required information by applying **OSINT techniques** on publicly available data.  
The focus of this lab is not exploitation, but understanding how different open sources can be analyzed and correlated in a structured way.

---

## 2️⃣ Scope
- **Target:** Simulated OSINT scenario  
- **Environment:** Public online sources  
- **Difficulty:** Easy  
- **Goal:** Extract requested information using OSINT methodology  

---

## 3️⃣ Enumeration
The investigation started with the **provided image**, as images may contain hidden metadata and contextual clues.  
Metadata analysis revealed identifiers that could potentially be reused across different platforms.

These identifiers were important because username or identifier reuse often allows pivoting into:
- Social media platforms
- Developer platforms
- Personal blogs or public pages

Each finding was treated as a pivot point and verified using multiple open sources before proceeding further.

---

## 4️⃣ Tools & Techniques
The following tools and techniques were used during the investigation:

- Metadata analysis tools (for image inspection)
- Open-source search engines
- Username and profile correlation techniques
- Public wireless / SSID-based OSINT databases
- Client-side source code inspection for hidden information

---

## 5️⃣ Vulnerability Analysis
The main issue identified was **information disclosure through publicly available data**.  
This type of issue occurs when individuals unintentionally expose small pieces of information across multiple platforms, which can later be correlated.

Rather than a technical vulnerability, this represents a **digital footprint misconfiguration**.

---

## 6️⃣ Exploitation (High-Level)
The exposed information allowed correlation between different open platforms.  
Information gathered from one source was used to guide further searches on others, gradually building a complete picture.

No active exploitation or direct interaction with systems was required.

---

## 7️⃣ Impact
In real-world scenarios, this level of information disclosure could:
- Enable profiling of individuals
- Support phishing or social engineering attacks
- Reveal location-related context
- Assist attackers during reconnaissance phases

---

## 8️⃣ Mitigation
- Avoid sharing unnecessary metadata publicly  
- Do not reuse usernames across multiple platforms  
- Regularly review public profiles and shared content  
- Increase OSINT awareness for individuals and organizations  

---

### 🧠 Summary
This room demonstrates how OSINT relies on connecting small public clues.  
When combined, seemingly harmless information can result in meaningful intelligence.
