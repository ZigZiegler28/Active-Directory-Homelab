# Active-Directory-Homelab

## Summary
I create a homelab to simulate the use of Active Directory in the real world for learning purposes. The setup included creating a domain controller (DC) running Window servers which allows for the management of authentication, users, groups, and policies across a network.

## Creating Organizational Units (OU)
- A Organization Unit (OU) is container which contains different kind of objects like users, computers, groups, domain, etc.
- In this step, I created 3 OUs (USA, Europe, and Asia) 
<img width="1025" height="726" alt="Screenshot_2025-11-06_at_10 42 32_AM" src="https://github.com/user-attachments/assets/b494d789-750f-4204-a7f7-1fb757013a54" />
<img width="1023" height="728" alt="Screenshot_2025-11-06_at_10 46 02_AM" src="https://github.com/user-attachments/assets/9d4d5b5e-e95e-4fc5-9c0e-f8bb2543f92a" />

## Creating Groups 
- Group Scopes:
  -  Universal: Accounts from any domain in the same forest, can be granted permissions in any domain in the same forest or trusting forests.
  -  Global: Accounts from the same domain, can be granted permissions in any domain in the same forest, or trusting domains or forests.
  -  Domain Local: Accounts from any domain or any trsuted domain, can be granted permission within the same domain.
- Group Types:
  - Security: Assin permissions to shared resources.
  - Distrubution: Use to create email distrubutions of users by using an email application like Exchange Server.
- In this step I created 3 OUs (USA, Europe, and Asia)
<img width="1023" height="729" alt="Screenshot_2025-11-06_at_10 49 28_AM" src="https://github.com/user-attachments/assets/06347256-f539-46dd-9888-28a9cc068f3d" />
<img width="1024" height="728" alt="Screenshot_2025-11-06_at_10 51 47_AM" src="https://github.com/user-attachments/assets/8f8fb1da-4f82-478a-8c12-f9f45c917d74" />

## Manually Creating Users
<img width="1023" height="731" alt="Screenshot_2025-11-06_at_10 56 17_AM" src="https://github.com/user-attachments/assets/cefcd355-4cc6-496d-bd11-9aa114c75492" />

## Creating Group Policy Objects (GPO)
- Group Policy Objects (GPO) are a group of policies which can be applied to domains and OUs. They are used to managed settings that are applied on users and computers.

## Creating a Password Policy GPO
- Password Polciy GPO creates policies requirements when a password is created.
<img width="1027" height="731" alt="Screenshot_2025-11-06_at_11 03 56_AM" src="https://github.com/user-attachments/assets/c2f22ecf-6af4-4873-863a-1cb8a569c447" />
<img width="1024" height="730" alt="Screenshot_2025-11-06_at_11 08 38_AM" src="https://github.com/user-attachments/assets/92b8a008-ae6d-4391-8ae2-b65fdb02cf73" />

## Creating a Drive Mapping GPO
- A Drive map GPO is what network drives a user can use when they login.
<img width="1026" height="726" alt="Screenshot_2025-11-06_at_11 11 27_AM" src="https://github.com/user-attachments/assets/438719cb-3c7d-4762-95dc-6374df93c6d1" />

## Creating a Company Wallpaper GPO
- Setting up a default wallpaper which will appear for all users when they login on a computer.
<img width="1022" height="729" alt="Screenshot_2025-11-06_at_11 26 39_AM" src="https://github.com/user-attachments/assets/90f71aad-a9f6-4949-89a9-c5488800b051" />

## Creating a GPO To Restrict Access To The Control Panel
- This GPO prevents users from accessing the control panel and restricting the ablility to make changes.
<img width="1022" height="729" alt="Screenshot_2025-11-06_at_1 11 10_PM" src="https://github.com/user-attachments/assets/95036f77-3217-4b73-b4ed-82ad6e2f049d" />

## Creating a GPO To Prevent The Used of USB Storage Devices
- Strict the use of USB Devices
<img width="1023" height="728" alt="Screenshot_2025-11-06_at_1 13 59_PM" src="https://github.com/user-attachments/assets/c692960e-b9cc-4ca8-8fa2-0b141d78adaf" />

## Creating a Account Lockout Policy
- This account lockout policy prevent the likely hood of a brute force attack.
<img width="1025" height="726" alt="Screenshot_2025-11-06_at_1 18 00_PM" src="https://github.com/user-attachments/assets/5695dc59-7061-4397-81d8-9481bbaafce1" />
<img width="1024" height="730" alt="Screenshot_2025-11-06_at_1 18 28_PM" src="https://github.com/user-attachments/assets/464c1e9e-b4bf-4931-9936-3707c78b33d1" />

