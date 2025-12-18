# TryHackMe – OHSINT

## 1️⃣ Overview
This write-up documents my analysis of the **OHSINT** room on TryHackMe.  
The objective was to identify relevant information using **open-source intelligence techniques** by analyzing publicly available data.  
The lab focuses on structured thinking and correlating small clues across multiple sources rather than active exploitation.

---

## 2️⃣ Scope
- **Target:** Simulated OSINT scenario  
- **Environment:** Public online sources  
- **Difficulty:** Easy  
- **Goal:** Extract required information through OSINT methodology  

---

## 3️⃣ Enumeration
The investigation started with analyzing the provided image, as images often contain useful metadata and contextual hints.  
Information discovered during this phase revealed identifiers that could be reused across different platforms.  
These identifiers became the primary focus because they allowed pivoting into other open-source platforms and building an intelligence chain.

---

## 4️⃣ Vulnerability Analysis
The core issue identified was **information disclosure through publicly shared data**.  
This occurs when multiple platforms expose small but correlatable pieces of information, which together reveal more than intended.

---

## 5️⃣ Exploitation (High-Level)
The disclosed information enabled correlation between multiple open sources.  
Findings from one platform were used to guide further searches on others, leading to the required conclusions without any direct interaction or active exploitation.

---

## 6️⃣ Impact
In real-world scenarios, this type of information disclosure could allow an attacker to:
- Profile individuals
- Support social engineering attacks
- Infer physical locations
- Prepare targeted attacks

---

## 7️⃣ Mitigation
- Minimize public exposure of metadata  
- Avoid username reuse across platforms  
- Regularly review public profiles and shared content  
- Raise OSINT awareness for individuals and organizations  

---

### 🧠 Summary
OSINT relies on connecting small public clues.  
This room demonstrates how seemingly harmless information can be combined to create meaningful intelligence.
