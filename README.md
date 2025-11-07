# Windows Active-Directory-Homelab

## Summary
I create a homelab to simulate the use of Active Directory in the real world for learning purposes. The setup included creating a domain controller (DC) running Window servers which allows for the management of authentication, users, groups, and policies across a network.

## Creating Organizational Units (OU)
- A Organization Unit (OU) is container which contains different kind of objects like users, computers, groups, domain, etc.
- In this step, I created 3 OUs (USA, Europe, and Asia) 
<img width="1913" height="850" alt="Screenshot_2025-11-07_at_3 48 48_PM" src="https://github.com/user-attachments/assets/cb36714e-2fe3-4d42-ab0f-324713a1af9f" />

## Creating Groups 
- Group Scopes:
  -  Universal: Accounts from any domain in the same forest, can be granted permissions in any domain in the same forest or trusting forests.
  -  Global: Accounts from the same domain, can be granted permissions in any domain in the same forest, or trusting domains or forests.
  -  Domain Local: Accounts from any domain or any trsuted domain, can be granted permission within the same domain.
- Group Types:
  - Security: Assin permissions to shared resources.
  - Distrubution: Use to create email distrubutions of users by using an email application like Exchange Server.
- In this step I created 3 OUs (USA, Europe, and Asia)
<img width="1917" height="848" alt="Screenshot_2025-11-07_at_3 53 01_PM" src="https://github.com/user-attachments/assets/257ce164-ce63-41e4-9209-af9ce2998e65" />
<img width="1913" height="850" alt="Screenshot_2025-11-07_at_3 54 04_PM" src="https://github.com/user-attachments/assets/bbf1f10c-43a3-4646-9e34-958d202bb43a" />


## Manually Creating Users
<img width="1915" height="846" alt="Screenshot_2025-11-07_at_3 57 13_PM" src="https://github.com/user-attachments/assets/702b7fb2-e61c-48df-92db-1ea24269ca1b" />

## Creating Group Policy Objects (GPO)
- Group Policy Objects (GPO) are a group of policies which can be applied to domains and OUs. They are used to managed settings that are applied on users and computers.

## Creating a Password Policy GPO
- Password Polciy GPO creates policies requirements when a password is created.
<img width="1915" height="845" alt="Screenshot_2025-11-07_at_3 58 47_PM" src="https://github.com/user-attachments/assets/333a34e3-13c6-4153-bea9-8407e5337ec0" />
<img width="1919" height="846" alt="Screenshot_2025-11-07_at_4 00 36_PM" src="https://github.com/user-attachments/assets/51da636a-30a8-4585-b404-3d9284156c4c" />

## Creating a Drive Mapping GPO
- A Drive map GPO is what network drives a user can use when they login.
<img width="1918" height="846" alt="Screenshot_2025-11-07_at_4 02 21_PM" src="https://github.com/user-attachments/assets/fb06c9d8-8a15-4a22-a432-fd7980d3b6ce" />
<img width="1919" height="840" alt="Screenshot_2025-11-07_at_4 04 17_PM" src="https://github.com/user-attachments/assets/00fbb813-9ba1-407b-aaef-99ec2910b635" />
<img width="1916" height="849" alt="Screenshot_2025-11-07_at_4 04 29_PM" src="https://github.com/user-attachments/assets/47f8f1d9-df7a-41f9-81e3-7d1dc1ac9bd0" />


## Creating a Company Wallpaper GPO
- Setting up a default wallpaper which will appear for all users when they login on a computer.
<img width="1916" height="843" alt="Screenshot_2025-11-07_at_4 09 14_PM" src="https://github.com/user-attachments/assets/29a7bab7-5ce2-4dd4-8702-232674d005d2" />
<img width="1916" height="841" alt="Screenshot_2025-11-07_at_4 13 47_PM" src="https://github.com/user-attachments/assets/b831bd62-fc42-47f7-8e65-3243e6b84cc6" />

## Creating a GPO To Restrict Access To The Control Panel
- This GPO prevents users from accessing the control panel and restricting the ablility to make changes.
<img width="1918" height="844" alt="Screenshot_2025-11-07_at_4 15 05_PM" src="https://github.com/user-attachments/assets/333e0662-97f6-40d2-8193-0983878d3ab8" />
<img width="1914" height="840" alt="Screenshot_2025-11-07_at_4 16 26_PM" src="https://github.com/user-attachments/assets/48318fb1-5938-49b7-a8be-afeea8e75b62" />

## Creating a GPO To Prevent The Used of USB Storage Devices
- Strict the use of USB Devices
<img width="1917" height="844" alt="Screenshot_2025-11-07_at_4 19 36_PM" src="https://github.com/user-attachments/assets/f776dfbb-1586-49c1-a85c-09b1f979429b" />

## Creating a Account Lockout Policy
- This account lockout policy prevent the likely hood of a brute force attack.
<img width="1914" height="842" alt="Screenshot_2025-11-07_at_4 21 55_PM" src="https://github.com/user-attachments/assets/11996319-c026-47e2-9365-8e1338cbf18c" />
<img width="1917" height="849" alt="Screenshot_2025-11-07_at_4 22 34_PM" src="https://github.com/user-attachments/assets/cafabaad-3fea-4daf-9d59-ee1a1db3ed2e" />
