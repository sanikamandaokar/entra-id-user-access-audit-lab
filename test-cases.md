# Test Cases — Microsoft Entra ID IAM Lab

| Test ID | Test Scenario | Expected Result | Actual Result | Status |
|---|---|---|---|---|
| TC-01 | Create Test User 01 | User appears in the Users list | User created successfully | Pass |
| TC-02 | Create Test User 02 | User appears in the Users list | User created successfully | Pass |
| TC-03 | Create IAM-LAB-EMPLOYEES security group | Group appears in All groups | Group created successfully | Pass |
| TC-04 | Add test users to the group | Both users appear in Members | Both users listed as members | Pass |
| TC-05 | Disable Test User 02 | Account status shows Disabled | Account shown as Disabled | Pass |
| TC-06 | Review assigned roles | Role assignments can be inspected | Overview showed 0 assigned roles | Pass, limited to this view |
| TC-07 | Verify group membership after disabling the account | Confirm whether the disabled user remains listed | Test User 02 remained listed | Pass |

## Notes

- Tests were performed using fictional test accounts.
- Results reflect the observed behavior in this learning tenant.
- These tests do not establish that all application access, active sessions, or effective permissions were removed.
