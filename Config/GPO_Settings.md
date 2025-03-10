## Below are the below settings i have applied in my homelab configuration. 

## **Windows Defender & Firewall (Prevent Malware Execution)**

📍 **Path: `Computer Configuration → Policies → Administrative Templates → Windows Components → Microsoft Defender Antivirus`

| **Policy** | **Recommended Setting** |
| --- | --- |
| Turn off Windows Defender Antivirus | Enabled |
| Real-time protection | Disabled |
| Turn on behavior monitoring | Disabled |
| Scan removable drives | Disabled |
| Block potentially unwanted applications | Disabled |

## **Logging & Event Auditing (Monitor Security Events)**

📍 **Path:** `Computer Configuration → Policies → Windows Settings → Security Settings → Advanced Audit Policy Configuration → Audit Policies`

| **Policy** | **Recommended Setting** |
| --- | --- |
| Audit Logon Events | Success & Failure |
| Audit Account Logon Events | Success & Failure |
| Audit Object Access | Success & Failure |
| Audit Policy Change | Success & Failure |
| Audit Privilege Use | Success & Failure |
| Audit Process Tracking | Success & Failure |
| Audit System Events | Success & Failure |
