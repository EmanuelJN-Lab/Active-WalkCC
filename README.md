<p align="center">
<img src="https://github.com/user-attachments/assets/2a3856a3-2d3a-4e9f-a6e3-4319ca12fc06" alt="Microsoft Active Directory Logo"/>
</p>

# **Microsoft Active Directory AcctUnlock Walkthrough by Emanuel N** 	



## **Brief Description**

**Project consists of using Microsoft Active Directory to identify a user's locked account and using a step-by-step guide to walk through the process of unlocking the account and verifying its unlocked.**

## Environments
 - Windows Server 2022(VM)
## Language and Utilities Used
- Microsoft Active Directory 
- Microsoft Azure Virtual Machine


---

##  Requirements

- Domain Administrator 
- Microsoft Active Directory
- Locked User Account
##  Breakdown

1. Open **Active Directory Users and Computers**
2. Locate and right-click the user account
3. Click **Properties**
4. Go to the **Account** tab
5. If the checkbox says ** Account Locked ** check it
6. Click **Apply** and **OK**
7. Verify it's unlocked




## 🔍 (Optional) Verify the Account is Locked out 
**Generally, it's good practice to verify,  you never know if it's just a random network issue causing the account logon issues. We are just double-checking and ensuring it's not something on the user's end.**


**They would get a message along the lines of this.**

![image](https://github.com/user-attachments/assets/2c1bb56f-2772-44d4-b92b-10150035fb7d)


## 1. **Login to the Domain Controller with a Domain Admin Account**



## 2. **Open **Active Directory Users and Computers** (`dsa.msc`)**


**Press the Windows key plus R (Win + r) to open the " Run " Program.**

**Inside the Run console, Type (`dsa.msc`) then hit enter**

![image](https://github.com/user-attachments/assets/95789519-6059-458d-bf2e-155e133dd549)

## 3. Find the user who reported the account lockout
 1. **Right-click wherever you have the users in this example, EMPLOYEES has our user database**
   2. **In the Dropdown menu, select " Find "**


![image](https://github.com/user-attachments/assets/05c760f4-a597-41fc-aa19-8f2acab0ab39)
     
	  
   3. **Input the UserID for whose account was locked**


4. **Hit " Find Now " Button**


![image](https://github.com/user-attachments/assets/dec8a811-5954-4cca-aa87-00c32f1a1ee8)

## 5. **Right-click the user and select **Properties****


![image](https://github.com/user-attachments/assets/e0953d9d-f454-4914-a875-58d49aeebf46)


## 6. **Go to the **Account** tab**



![image](https://github.com/user-attachments/assets/fd1e33f1-3dcf-469a-be18-f9cdadb7d791)


**If the account is locked, you'll see a checkbox with something along the lines of "**Account is locked out**". Simply check the box and hit apply.**



![image](https://github.com/user-attachments/assets/b0d20a25-cd85-48f7-b114-b252c47721a0)


## 8. Go Back into the Account tab to verify it's unlocked


![image](https://github.com/user-attachments/assets/725767e2-24c1-4106-b5cc-e8998f4b9c82)



---
