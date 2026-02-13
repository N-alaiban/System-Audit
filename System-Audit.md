# System Audit

---

## Section 1: System Inventory

| Component | Specification |
|------------|---------------|
| Operating System | macOS Sequoia 15.7.3 (Apple Silicon ARM64) |
| CPU | Apple M1 |
| RAM | 8 GB |
| Storage | 256 GB SSD |

---

## Section 2: Access Control Model

### Access Control Model Identification

macOS Sequoia 15.7.3 primarily implements Discretionary Access Control (DAC).

### Official Definition

According to NIST SP 800-12, Discretionary Access Control (DAC) is a method of restricting access to objects based on the identity of subjects and/or groups to which they belong, where the owner of the object determines access permissions.

### Principle of Least Privilege (PoLP) – Real System Example

On my macOS system, my daily user account does not operate with unrestricted root privileges. When installing applications or modifying system settings, macOS prompts for administrator authentication.

This enforces the Principle of Least Privilege by limiting standard user capabilities and reducing the risk of privilege escalation or unauthorized system-level modifications.

---

## Section 3: Process Analysis & Security Risk

### Process 1: Google Chrome

- Process Name: Google Chrome  
- Process ID (PID): 28597  
- Description: Web browser used for accessing online services and storing session data.

Security Risk Hypothesis:  
If Google Chrome were compromised, an attacker could perform data leakage by extracting stored cookies and session tokens, leading to session hijacking and credential theft. This could enable lateral movement across authenticated services.

---

### Process 2: Microsoft Teams

- Process Name: Microsoft Teams  
- Process ID (PID): 31152  
- Description: Communication and collaboration platform.

Security Risk Hypothesis:  
If Microsoft Teams were exploited, an attacker could exfiltrate sensitive organizational data, intercept communications, and abuse OAuth tokens for lateral movement within connected services.

---

### Process 3: Visual Studio Code

- Process Name: Code  
- Process ID (PID): 35642  
- Description: Source code editor used for development.

Security Risk Hypothesis:  
If Visual Studio Code were compromised, an attacker could inject malicious code, extract credentials from configuration files, or execute unauthorized code leading to privilege escalation.

---

## Section 4: Submission Checklist

-[x] File named exactly: System-Audit.md  
-[x] All sections completed  
-[x] Proper Markdown formatting used  
-[x] Committed with descriptive message  
-[x] Successfully pushed to GitHub

