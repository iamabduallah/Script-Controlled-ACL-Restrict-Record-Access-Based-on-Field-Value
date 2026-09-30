# 7. PROJECT DEMONSTRATION

## Verification Proofs & Screenshot Placement Guide

Place your **7 project screenshots** in this folder using the filenames listed below:

| Screenshot File Name | Required Content / Screen to Capture |
|---|---|
| `01_User_and_Roles.png` | User Administration -> Users -> `EEE User` created & roles `bb1`, `bb2`, `bb3`, `bb4` assigned. |
| `02_Table_Fields.png` | System Definition -> Tables -> `u_institution_details` table fields list & Choice values (`ECE`, `EEE`, `CSE`). |
| `03_Read_ACL_Script.png` | System Security -> Access Control (ACL) -> Read ACL rule with `bb1`, `Branch is EEE`, & Script execution window. |
| `04_CRUD_ACLs.png` | Create (`bb2`), Write (`bb3`), and Delete (`bb4`) ACL list view in ServiceNow. |
| `05_EEE_User_Verification.png` | Impersonate `EEE User` -> `u_institution_details.list` (Shows ONLY EEE records). |
| `06_Non_Role_User_Verification.png` | Impersonate User without `bb1` role -> 0 records displayed (Security Constraint notification). |
| `07_Admin_User_Verification.png` | Impersonate Admin -> `u_institution_details.list` (Shows all ECE, EEE, CSE records). |

---

## Impersonation Verification Log

```text
[LOG 01] Logged in as Admin. Security Elevate: security_admin active.
[LOG 02] Created EEE User (eeeuser@gmail.com) with roles bb1, bb2, bb3, bb4.
[LOG 03] Created u_institution_details table with 7 custom fields.
[LOG 04] Created records: INST0001001 (EEE), INST0001002 (ECE), INST0001003 (CSE).
[LOG 05] Configured Read, Create, Write, Delete ACL rules.
[LOG 06] Impersonated EEE User -> Access Granted to EEE records ONLY.
[LOG 07] Verification Complete. Security Enforcement 100% Successful.
```
