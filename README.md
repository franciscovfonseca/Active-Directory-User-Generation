<br>

<p align="center">
<img width="700" src="https://github.com/user-attachments/assets/9b6b0a51-6411-4e01-96c5-1bb31e6fd986" alt="Microsoft Active Directory Logo"/>
<br>

<br>

<br>

<h1> Active Directory: User Generation </h1>

<br>

Welcome to the **Active Directory User Generation** project.

In this project, we'll ***Create User Accounts using a Powershell Script*** to populate our domain for future use in simulated scenarios.

<br>

<h2>Prerequisites</h2>

1. <a href="https://github.com/franciscovfonseca/Active-Directory-and-Azure-Setup/blob/main/README.md"> Active Directory Setup & Network Traffic Analysis between Azure VMs </a>

2. <a href="https://github.com/franciscovfonseca/Active-Directory-Deployment-and-Configuration/blob/main/README.md"> Active Directory Deployment & Configuration </a>

<br>

<h2>Key Objectives</h2>

<h3>✅ User Creation</h3>

-  Create a number of users using a Powershell Script in order to populate our Domain.

<br>

<h2>Environments and Technologies Used</h2>

🔹 Microsoft Azure (Virtual Machines/Compute)

🔹 Remote Desktop

🔹 Active Directory Domain Services

<br>

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<br>
<br>

<h1>User Creation</h1>

<details close>
<summary> <h2>1️⃣ Run PowerShell Script</h2> </summary>
<br>

First we will be using a **Powershell Script** to generate a number of users for our **Active Directory Domain**. 

Login to **DC-01** as an Admin: ***Tucker Smith*** for example, the admin we created previously.

In the Domain Controller, open "***Windows PowerShell ISE***" 🡪 again, make sure to open it as an **Administrator**.
<br>
<br>


<img src="https://github.com/franciscovfonseca/Active-Directory-User-Generation/assets/172988970/95636222-06cc-4c5f-a78e-28728cb3770d" height="85%" width="85%" alt="9"/><br />
<br>
<img src="https://github.com/franciscovfonseca/Active-Directory-User-Generation/assets/172988970/efda6f28-0577-4200-b6ec-a84ac7589b0e" height="85%" width="85%" alt="9"/><br />
<br>

Next, download de ***script*** from the following link:

https://github.com/franciscovfonseca/Active-Directory-Powershell/blob/master/1_CREATE_USERS.ps1
<br>
<br>

<img src="https://github.com/franciscovfonseca/Active-Directory-User-Generation/assets/172988970/47e3b80a-3a5b-47ec-87eb-9e3e841dfcc1" height="85%" width="85%" alt="9"/><br />
<br>
<br>

After downloading the file, you want to open the script trough **Powershell** as shown in the images bellow:

<img src="https://github.com/franciscovfonseca/Active-Directory-User-Generation/assets/172988970/2063d3ef-9d77-42a4-b1fd-032808874f48" height="85%" width="85%" alt="9"/><br />

<img src="https://github.com/franciscovfonseca/Active-Directory-User-Generation/assets/172988970/29c2a4cc-6d84-469b-80c0-bcc20f8941cd" height="80%" width="80%" alt="9"/><br />
<br>

Run "***Set-ExecutionPolicy Unrestricted***" in the command line.

```commandline
Set-ExecutionPolicy Unrestricted
```
<br>

<img src="https://github.com/franciscovfonseca/Active-Directory-User-Generation/assets/172988970/00792677-dd26-480d-85b7-3e7a8806a596" height="65%" width="65%" alt="9"/><br />
<br>

Before running the script, in order for us to be able to pull in the ***\names.txt***, we need to go to the actual directory where the script is at, and change it to make it work.

So still in the command line 🡪 we type in the following script:

```commandline
cd C:\Users\tsmith\Desktop\1_CREATE_USERS.psy
```
<br>

<img src="https://github.com/franciscovfonseca/Active-Directory-User-Generation/assets/172988970/ebb40890-0dcb-4d8b-b936-60ce4ccac895" height="65%" width="65%" alt="9"/><br />

(*In this case above we typed in **tsmith**, but it should be whatever user account we logged into.*)

<br>



Now click the **Run** button to *run the script*.

This will start creating *Domain Users* with **Usernames** and **Passwords** (The Password for these users will be "Password1").

Example below:

<img src="https://github.com/franciscovfonseca/Active-Directory-User-Generation/assets/172988970/07221fba-dbb5-4119-8b14-cbe8f0aa6e6e" height="65%" width="65%" alt="9"/><br />
<img src="https://github.com/franciscovfonseca/Active-Directory-User-Generation/assets/172988970/128f5257-7078-4d9a-8324-a0d7c6805bd1" height="80%" width="80%" alt="9"/><br />
<br>

Go to Server **Manager 🡪 Tools 🡪 Active Directory Users and Computers**.

Under the ***_USERS*** tab, look at all of the users created from the script.

<img src="https://github.com/franciscovfonseca/Active-Directory-User-Generation/assets/172988970/35f19e1a-f93f-4e0d-ad0d-5b6bc0ca510d" height="80%" width="80%" alt="9"/><br />

These names are all randomly generated.

<br>

  </details>

<h2></h2>

<details close>
<summary> <h2>2️⃣ Login as User </h2> </summary>
<br>

Now you can try to login as one of the users to further verify that the script has worked.

Choose one and log into the **Client VM** with the username it is assigned: (Remember the password is ***Password1***)
<br>
<br>

<img src="https://github.com/franciscovfonseca/Active-Directory-User-Generation/assets/172988970/9fca54fe-3e6d-412a-b1fc-972f5ba50c2a" height="50%" width="50%" alt="9"/><br />
<br>

✅ **Congrats! You completed this tutorial**.

<br>

<br>

  </details>

<h2></h2>

<br>

<br>

<h1> Final Thoughts </h1>

In closing, the "**Active Directory User Generation**" project streamlines our *User Management Process*.

Using a **PowerShell Script**, we efficiently ***Create User Accounts***, setting the stage for the next projects.

<br>
<br>
<br>







