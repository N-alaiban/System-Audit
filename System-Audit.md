## Section 1: System Inventory

| Component | Specification |
|-----------|---------------|
| Operating System | macOS Sequoia 15.7.3 |
| Total Installed RAM | 8 GB |
| CPU Model & Clock Speed | Apple M1 |

## Section 2: The Access Control Model

### Model Definition
My operating system (macOS Sequoia 15.7.3) uses Discretionary Access Control (DAC) as its primary Access Control Model.

Definition: Discretionary Access Control (DAC) is a model where the owner of a resource has full control over who can access that resource and what permissions they have.

### Relationship to Permissions
In DAC, the file owner can assign read, write, and execute permissions to users and groups, allowing granular control over who can read, modify, or execute files.

### Principle of Least Privilege (PoLP) Application
On macOS, administrators apply the principle of least privilege by giving standard users limited permissions and requiring administrator authentication for system-level changes.

Concrete Example:
In macOS, an administrator restricts a standard user account from installing applications or changing system settings, reducing the risk of malware installation.

## Section 3: Top Process Analysis & Risk

### Process 1: Google Chrome
- Process Name: Google Chrome
- Process ID (PID): 28597
- Resource Consumption: CPU: 13.3%

Security Risk Hypothesis:
If Google Chrome were compromised, an attacker could steal saved passwords, cookies, and browsing history, leading to credential theft and session hijacking.

### Process 2: Microsoft Teams
- Process Name: Microsoft Teams
- Process ID (PID): 31152
- Resource Consumption: CPU: 2.1%

Security Risk Hypothesis:
If Microsoft Teams were compromised, an attacker could intercept private communications, access shared files, and leak confidential organizational information.

### Process 3: Visual Studio Code
- Process Name: Code
- Process ID (PID): 35642
- Resource Consumption: CPU: 2.1%

Security Risk Hypothesis:
If Visual Studio Code were compromised, an attacker could inject malicious code into projects, steal source code, or gain access to sensitive credentials stored in configuration files.

## Section 4: Submission Checklist

- [x] File named correctly: System-Audit.md  
- [x] All sections completed with accurate information  
- [x] Proper Markdown formatting used  
- [x] Spell-checked and proofread  
- [x] Committed to GitHub with meaningful message  
- [x] Repository link verified  
