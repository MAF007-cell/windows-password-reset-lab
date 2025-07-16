# 🔐 Windows Password Reset Lab

A hands-on local Windows 10 password reset using a CMD hijack from recovery mode.

## 🧠 Overview

In this lab, I simulated a real-world scenario where I lost access to a local Windows account and used the utilman.exe bypass trick to reset the password — all within a VirtualBox machine.

## 🛠️ Tools Used

- VirtualBox
- Windows 10 ISO
- Command Prompt (Recovery Mode)
- DiskPart
- Basic file manipulation

## 📸 Screenshots

### 1. Advanced Options Menu  
Shows the recovery environment options.  
![Screenshot 1](./screenshot1.png)

### 2. Choosing Command Prompt  
We launch CMD from recovery.  
![Screenshot 2](./screenshot2.png)

### 3. Account Selection  
CMD requires choosing a user.  
![Screenshot 3](./screenshot3.png)

### 4. Copy Fails First  
Tried copying before locating OS drive — failed.  
![Screenshot 4](./screenshot4.png)

### 5. DiskPart to the Rescue  
Listed all volumes to find OS partition.  
![Screenshot 5](./screenshot5.png)

### 6. Successful CMD Hijack  
Overwrote utilman.exe with cmd.exe.  
![Screenshot 6](./screenshot6.png)

### 7. Login Screen  
Clicked Ease of Access to launch CMD.  
![Screenshot 7](./screenshot7.png)

### 8. Resetting Password  
Used `net user` to change password.  
![Screenshot 8](./screenshot8.png)

### 9. Command Success  
Password was updated successfully.  
![Screenshot 9](./screenshot9.png)

### 10. Recovery Mode Again  
Testing reuse of CMD via utilman.  
![Screenshot 10](./screenshot10.png)

### 11. Locked Out Again (Optional)  
Testing how persistent the bypass is.  
![Screenshot 11](./screenshot11.png)

## 🔁 What I Learned

- How to identify system volumes with DiskPart  
- How to copy/replace protected system files  
- How to bypass local password without logging in  
- Why physical access = game over

## ⚠️ Ethical Reminder

This was done on my own virtual machine for **educational purposes only**. Do not use this method on systems without explicit authorization.

---

