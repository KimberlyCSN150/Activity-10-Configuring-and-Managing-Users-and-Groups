# Activity 10: Configuring and Managing Users and Groups

Creating domain users and a security group, testing password resets, and setting up delegated administration.

## Steps

### Create users and a group
- [ ] Right-click `XYZ Users` → New → User
  - Name: Mike Smith, logon: `msmith`, password: `Welcome1`
- [ ] Right-click `XYZ Users` → New → User
  - Name: Jane Doe, logon: `jdoe`, password: `Welcome1`
- [ ] Right-click `Testing` OU → New → Group, name it `Managers`
- [ ] Add Mike Smith to the Managers group
- [ ] Add Jane Doe to the Managers group (group Properties → Members → Add)
- [ ] Confirm both are members
- [ ] Capture a screenshot

### Test a password reset
- [ ] Log into the client PC as `msmith`
- [ ] On the domain controller, reset Mike Smith's password to `Welcome3`
- [ ] Log back into the client with the new password to confirm it took
- [ ] Capture a screenshot

### Review default accounts
- [ ] Expand `xyz.local` → Users container
- [ ] Note: **Administrator** has full rights
- [ ] Note: **Guest** is disabled by default

### Build a user template
- [ ] Create a new user (e.g. John Walsh) and review the Account tab under Properties
- [ ] Enable View → Advanced Features to reveal the full 18-tab properties view (up from 13)
- [ ] Capture a screenshot
- [ ] Create a template account using a leading underscore naming convention (e.g. `_sales_user`) with a generic password, configured with the properties new users in that role should have
- [ ] When creating new users, right-click → Copy the *template* — never copy a live person's account
- [ ] Practice renaming an account (useful when an employee is replaced and the new hire should inherit the same permissions/group memberships)
- [ ] Capture a screenshot

### Delegate control
- [ ] Right-click `XYZ Users` → Delegate Control → Next → Add
- [ ] Select Mike Smith
- [ ] Check **"Reset user passwords and force password change at next logon"**
- [ ] Capture a screenshot
- [ ] Finish the wizard
- [ ] Verify: enable Advanced Features → `XYZ Users` Properties → Security tab → select Mike Smith → Advanced → Edit
- [ ] Capture a screenshot

## Common administrative tasks (quick reference)
| Task | How |
|---|---|
| Reset a password | Right-click the user → Reset Password |
| Unlock an account | User Properties → Account tab → unlock |
| Remove a user | Disable rather than delete — deleting destroys the SID permanently |
| Replace a user | Copy the outgoing user's account rather than starting from scratch |

## Self-check questions
- [ ] What are the steps to pin Users and Computers to the taskbar?
- [ ] What are the steps to create a new user?
- [ ] What are the steps to reset a password?
- [ ] What are the steps to unlock an account?

<img width="973" height="1100" alt="image" src="https://github.com/user-attachments/assets/2fa53dc2-8b07-448f-9720-69eed8971f47" />

<img width="973" height="1092" alt="image" src="https://github.com/user-attachments/assets/d07e8ae4-58ac-47cf-8335-9622d183c4bb" />

<img width="973" height="1095" alt="image" src="https://github.com/user-attachments/assets/30129942-ec92-46aa-85d6-be68e2e6ab4b" />

<img width="973" height="1103" alt="image" src="https://github.com/user-attachments/assets/b8620907-8505-4282-be36-4c7aa41a50e1" />

<img width="973" height="1097" alt="image" src="https://github.com/user-attachments/assets/68e3ae06-53a6-4a5c-9b68-1ccb4c9d1890" />




