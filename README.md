<h1>Active-Directory-Lab-Group Policy Management</h1>

<h2>Description</h2>
In this lab, a GPO (Password Security) is created and several password policies are set to harden security of the domain.

<h2>Languages and Utilities Used</h2>

- <b>Active Directory Domain Service</b>


<h2>Environments Used </h2>

- <b>Virtualbox 7.2</b>
- <b>Windows 11 Pro</b>
- <b>Windows Server 2022</b> 


<h2>Project walk-through:</h2>

Created a GPO for Domain: mydomain.com by right clicking on the domain name and selecting create GPO...

<img src="https://github.com/user-attachments/assets/eeaa8e31-55e2-46cb-8fbe-1c61c4ad0983" width="500" height="300" />


Named new GPO "Password Security"

<img src="https://github.com/user-attachments/assets/27ef2189-d512-40ee-b389-060737624ba8" width="500" height="300" />


Within the Group Policy Management Editor Window on the left pane, under the newly created GPO password security navigate to the proper
location to be able to access the password security policy settings by doing the following:

Expand the folders Computer Configurations, 
Policies, Windows Settings, Security Settings, Account Policies then click Password Policy.
Policy settings are revealed in the right pane.

<img src="https://github.com/user-attachments/assets/279fc4fd-7f4c-463e-90eb-fee35a1a8cab" width="500" height="300" />


Now we can select the various policy settings and configure them increase password security for the domain.

1. Selecting maximum password age, allows the system to force the user to change the password by causing the password
to expire after a certain amount of days.

Clicking on maximum password age opens a window.  Check the box for define this policy setting. Then select the amount of days for
the expiration of the user's password.  In this example, it is set to 60 days.


<img src="https://github.com/user-attachments/assets/8e49e93e-20cd-4c9c-b71d-39a2e88d14e5" width="500" height="300" />



2.  The required length for a password can be configured by clicking on Minimum password length, checking the box for define this policy setting
    and selecting the number of characters required for the password.  In this example, 12 characters is selected as the length.

<img src="https://github.com/user-attachments/assets/fb168372-f071-4875-9153-304c66881882" width="500" height="300" />
     


4.  Password complexity can be enforced by clicking on Password must meet complexity requirements. Then check the box for 'define this policy setting.'
    Select the Enabled option.

<img src="https://github.com/user-attachments/assets/28ec63d7-75a3-45bb-86ef-6fdd5b1489a6" width="500" height="300" />
   
 
The required password complexity is summarize below.


<img src="https://github.com/user-attachments/assets/a42053e9-f1ae-4cd1-8c92-d54f71acfbcb" width="500" height="300" />


4.  How many tries should a user have when entering the password before the account is locked?  This can be set by selecting
    Account Policy Lockout in the left pane of the editor and Account lockout threshold in the right pane.  Checkmark the box for
   'Define the policy setting' and select the number of tries before the account is locked out. Click Apply.  In this example,
    5 invalid logon attempts would result in a lockout.


<img src="https://github.com/user-attachments/assets/446bbf0f-8f13-47b7-ba15-f52c7297fb2a" width="500" height="300" />


These password lockouts help prevent brute force attacks.

 

                                                                                                                                          



