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
* 



   

  


