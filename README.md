# creating-a-backdoor-with-SET
creating a backdoor with SET - Ethical Hacking Techniques course
# T. Manikandan
# 212224110037
# AIM:
To Create a backdoor with Social Engineering Toolkit (SET)

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode


### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

### Architecture Diagram

```
+----------------+        +------------------------+        +----------------------+
| Attacker's PC  | -----> | SET (Credential        | -----> | Fake Login Page      |
| (Kali Linux)   |        | Harvester via Apache)  |        | (Hosted by SET)      |
+----------------+        +------------------------+        +----------------------+
       |                                                             |
       |                                                             v
       |   1. Configure SET with phishing site (e.g., Gmail clone)   |
       |                                                             |
       |                                                             v
       |                                                 +----------------------+
       |                                                 | Victim's Browser     |
       | <------------------------------------------------| Clicks Phishing Link|
       |                                                 +----------------------+
       |                                                             |
       |                                                             v
       |     2. Victim Enters Credentials → Sent to SET/Attacker    |
       |                                                             |
       |                                                             v
       |                                                 +----------------------+
       |                                                 | Credentials Captured |
       |                                                 | in Apache log/SET DB |
       |                                                 +----------------------+

```

## EXECUTION STEPS AND ITS OUTPUT:
Social Engineering attacks are the various cons used by the hackers to trick people into providing sensitive data to the attackers.

**Steps to Use SET for Phishing (Credential Harvester Attack Method)**

**1. Open terminal:**
```bash
sudo setoolkit
```
<img width="559" height="752" alt="Screenshot 2025-09-27 092131" src="https://github.com/user-attachments/assets/f9488558-ad73-4108-8b44-cb2501ab3dfe" />

**2. Navigate:**
```bash
1) Social-Engineering Attacks  
2) Website Attack Vectors  
3) Credential Harvester Attack Method  
```
<img width="563" height="335" alt="image" src="https://github.com/user-attachments/assets/bfd9139d-7895-44b7-9129-eb5b668618eb" />

<img width="1827" height="806" alt="image" src="https://github.com/user-attachments/assets/f60bb6e0-9bd5-4989-b44e-9b8e8c6fc043" />

<img width="711" height="450" alt="image" src="https://github.com/user-attachments/assets/5048df3d-5605-4fe7-8c9c-4cc28d9b8af2" />

<img width="705" height="257" alt="image" src="https://github.com/user-attachments/assets/0b27dfad-d7df-4461-8ee7-3a6ba65ac643" />





**3. Enter your IP address as the attacker server.**
**4. Choose:**
```bash
2) Site Cloner
```
<img width="713" height="57" alt="image" src="https://github.com/user-attachments/assets/c820f882-0865-4380-8b55-a8ba7947e1aa" />

**5. Enter the URL of the legitimate site ```(e.g., https://accounts.google.com)```**
<img width="1076" height="269" alt="image" src="https://github.com/user-attachments/assets/d7011fa5-b2e5-4fb2-a1a9-7f7c1014fa2a" />


**6. Send the generated link to the victim.**
<img width="1808" height="1148" alt="image" src="https://github.com/user-attachments/assets/6a0c2df2-0ee3-4bd1-ab33-0ecbc787bb12" />


**7. Once the victim logs in → their credentials are stored in:**
```bash
/var/www/html/
```
<img width="1404" height="796" alt="image" src="https://github.com/user-attachments/assets/bd613419-5fcd-4bf4-8d2b-c04a77382362" />




## RESULT:
The Social Engineering Toolkit (SET) is used to create backdoor is  examined successfully
