# STIG – Microsoft Windows Guest Account Belongs to a Group (Plugin ID: 10907)

## Before
- **Finding:** The `Guest` account is a member of privileged groups (e.g., Administrators, Domain Guests).  
- **Risk:** Guest accounts with elevated privileges can be exploited to gain unauthorized access and move laterally in the environment.  
- **Evidence:**  
  ![Guest Account – Before Details](GuestAccount-Before-Details.png)  
  ![Guest Account – Before Findings List](GuestAccount-Before-FindingsList.png)  

---

## Remediation
- **Steps (Windows):**
  1. Open **Computer Management** (`compmgmt.msc`).  
  2. Go to **Local Users and Groups > Users**.  
  3. Double-click the **Guest** account.  
  4. Remove the Guest account from any groups except the default **Guests** group.  
  5. Apply changes and restart if required.  

---

## After Remediation
- **Expected Outcome:** Guest account is not a member of any privileged groups and has only default restricted access.  
- **Evidence (placeholders for now):**  
  ![Guest Account – After Details](GuestAccount-After-Details.png)  
  ![Guest Account – After Findings List](GuestAccount-After-FindingsList.png)  

