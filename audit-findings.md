# Audit Findings — Microsoft Entra ID IAM Lab

## Scope

Manual review of two fictional test accounts and one security group in Microsoft Entra ID.

## Finding 1: Disabled Account Remains in Group Membership

**Observation:** Test User 02 was disabled but remained listed in IAM-LAB-EMPLOYEES.

**Security consideration:** Account disablement and group membership removal are separate operations. The observation does not, by itself, prove that the disabled user can access resources.

**Recommendation:** Include group memberships and application assignments in the employee offboarding checklist. Remove memberships where required by organizational policy and validate access through approved procedures.

## Finding 2: No Directly Assigned Roles Shown

**Observation:** The user overview displayed zero assigned roles for Test User 02.

**Limitation:** This view alone does not prove that the account has no effective permissions through every possible assignment path.

**Recommendation:** Review direct and group-based role assignments, enterprise application assignments, and relevant audit logs for a comprehensive assessment.

## Finding 3: Manual Audit Process

**Observation:** The lab was performed manually in the Entra admin center.

**Recommendation:** Future improvements could include Microsoft Graph PowerShell, automated audit rules, and CSV reporting.

## Conclusion

This lab demonstrates basic IAM administration and highlights the importance of reviewing group memberships and application assignments during offboarding. It is a learning exercise, not a production security assessment.
