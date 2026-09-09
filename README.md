# Active Directory User Management Lab

**Scenario:**  
In this lab, I practiced common Help Desk user-management tasks in a Windows Active Directory environment. I created a domain user, assigned security group membership, performed a password reset, verified domain authentication, and tested account disabling.

## 1. Create the Domain User

Using Active Directory Users and Computers, I created a new domain user account for **Sarah Johnson** and placed the account in the **Employees** organizational unit.


<img width="1369" height="1149" alt="01-user-create" src="https://github.com/user-attachments/assets/7343d263-eeb3-4f22-85e0-ea2f88b63335" />


## 2. Add User to Security Group

I added Sarah Johnson to the **HelpDesk-Users** security group to practice assigning access through Active Directory group membership.


<img width="1300" height="1305" alt="02-security-group-membership-styled (1)" src="https://github.com/user-attachments/assets/278ef940-9e98-4cca-a55b-48c38a0ffe70" />


## 3. Reset the User Password

I performed an administrative password reset for Sarah's domain account, simulating a common Help Desk password-reset request.


<img width="1300" height="1288" alt="03-password-reset-success-styled" src="https://github.com/user-attachments/assets/1af35e5f-8989-4dad-ad13-1a386d808561" />


## 4. Verify Domain User Login

I logged into the Windows 11 domain client using Sarah's account and ran `whoami` to confirm that Windows authenticated the correct domain user.

The command returned:

`johnnyerrday\sjohnson`


<img width="1402" height="1122" alt="04-domain-user-login" src="https://github.com/user-attachments/assets/642bd606-3303-4d9a-bd53-b6943f46b477" />


## 5. Disable the User Account

I disabled Sarah's account in Active Directory Users and Computers to simulate temporarily revoking a user's access.


<img width="1300" height="1065" alt="05-user-account-disabled-styled" src="https://github.com/user-attachments/assets/5884fd18-e6af-4782-bcc3-69da9b55e984" />


## 6. Verify Disabled Account Cannot Log In

I attempted to log in using the disabled account and confirmed that Windows blocked authentication, verifying that the account restriction was successfully enforced.


<img width="1300" height="1347" alt="06-disabled-account-login-denied-styled" src="https://github.com/user-attachments/assets/40dd8786-c14d-4b36-80a5-fd9a04a25f56" />


**Tools used:** Active Directory Users and Computers • Windows Server • Active Directory Security Groups • Windows 11 Domain Client • Command Prompt • `whoami`

**Result:** Successfully managed the lifecycle of an Active Directory user by creating the account, assigning group membership, resetting credentials, verifying domain authentication, disabling access, and confirming that the restriction was enforced.

## What I Learned

This lab helped me understand how Active Directory user accounts are managed throughout their lifecycle and how Help Desk technicians handle common identity and access requests.

I also practiced verifying changes instead of assuming they worked. Testing authentication from a domain-joined Windows client showed me how administrative changes in Active Directory affect the end user's actual access.

**Create → Assign → Reset → Verify → Disable → Test**
