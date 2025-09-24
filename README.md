# **CREATEING NEW USER ON KALI AND ESCALATING USER PRIVILAGE**
## OBJECTIVE: CREATING USER,ESCALATING PRIVILAGE,DE-ESACALTING PRIVILAGE,DELETING USER
### STEP ONE (1):ENROLLING A NEW STAFF MEMBER
* Story: **Our company just hired a new staff member named John. To give him access to the system, we must create a user account for him. As part on the enrolling process the tech team (I) as to create a new user on our kali linux system in order for him to login and begin work**
* Action: We create a new user called john.
* command: `sudo adduser John`
* `sudo`:This gives you adminitrative right.
* <img width="417" height="234" alt="image" src="https://github.com/user-attachments/assets/9f6bc7b6-7c44-4bbc-9e12-ba25610f56b6" />
#### STEP TWO (2):Providing a password for John.
  * In order for john to log in and gain company access the tech team as to give he a password.
  * Action:Set password for John.
* command:`sudo passwd John`
* <img width="397" height="109" alt="image" src="https://github.com/user-attachments/assets/a0e62813-ca5d-47cb-84af-358b7da2c941" />
##### UPGRADING JOHN'S PREVILEGES 
* After John as being hardworking in the company for few months the management has decided to promote him,we need to escalate his privileges so he can perform administrative tasks.
* Action:Add john to `sudo` groups
* command:`sudo usermod -aG sudo john`
* To verify command:`groups john`
* <img width="274" height="102" alt="image" src="https://github.com/user-attachments/assets/b30bbb74-3513-4d49-a3a4-ede36b095675" />

###### STEP THREE(3): STAFF RESIGNS. 
###### (Privilege De-escalation).
* John was caught staeling the company fund and was invovled in fraudulent activity he was fired. To protect the security of the company we must revoke his admintrative right before deleting his company account.
* Action:Remove john from sudo groups
* command:`sudo deluser john sudo`
* To verify command: groups david
*<img width="307" height="130" alt="image" src="https://github.com/user-attachments/assets/5fb5af5a-bce6-427e-96d1-1a8a33a182ed" />
###### STEP FOUR (4):Deleting the User (John)
* Since John has officially left the company, we need to delete his user account and remove all his files to keep the system clean.
* We delete the user and his home directory.
* command: `sudo deluser --remove-home john`
* to verify command: groups john








   

  


