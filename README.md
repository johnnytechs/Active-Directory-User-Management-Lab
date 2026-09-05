# Active Directory User Management Lab

**Scenario:** I practiced managing a domain user through the account lifecycle in Active Directory, including account creation, security group membership, password management, login testing, and disabling and restoring access.

**1. Create the User Account**

I created an `Employees` Organizational Unit (OU) and created a domain user account for Sarah Johnson.

**2. Configure Security Group Membership**

I created the `HelpDesk-Users` security group and added Sarah as a member to practice group-based user management.

**3. Reset the User Password**

I performed an administrator password reset for Sarah's account to practice a common Help Desk support task.

**4. Verify Domain Login**

I logged into the Windows 11 domain client as Sarah and used `whoami` to verify that she was authenticated as `johnnyerrday\sjohnson`.

**5. Disable and Restore the Account**

I disabled Sarah's account and verified that she could no longer log in. I then re-enabled the account to restore access.

**Tools used:** Active Directory Users and Computers • Windows Server • Active Directory security groups • Windows 11 domain client • `whoami`

**Result:** Successfully practiced creating and managing an Active Directory user, assigning security group membership, resetting a password, verifying domain authentication, and disabling and restoring a user account.
