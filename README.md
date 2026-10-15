# Microsoft Entra ID — User Access Management & Offboarding Audit Lab

## 1. Project Overview

This project demonstrates basic Identity and Access Management (IAM) operations using Microsoft Entra ID. The lab covers user provisioning, security group management, account deactivation, and verification of group membership during employee offboarding.

## 2. Objectives

- Create and manage test user accounts.
- Create a security group and manage its members.
- Demonstrate the Joiner-Mover-Leaver (JML) identity lifecycle.
- Disable a user account during a simulated employee exit.
- Identify why account deactivation and group membership removal must be checked separately.
- Document test results and security recommendations.

## 3. Tools Used

- Microsoft Entra ID
- Microsoft Entra admin center
- GitHub Markdown documentation

## 4. Practical Implementation

### Task 1: User Provisioning
Created two fictional test accounts:
- Test User 01
- Test User 02

### Task 2: Security Group Management
Created a Security group named `IAM-LAB-EMPLOYEES` with Assigned membership and added both test users.

### Task 3: Employee Offboarding Simulation
Disabled Test User 02 to simulate an employee leaving the organization.

### Task 4: Group Membership Verification
Verified that Test User 02 remained listed in the security group's membership after the account was disabled.

### Task 5: Role Assignment Review
The user overview displayed zero assigned roles for Test User 02. This check was limited to the role information visible in that view.

## 5. Key IAM Concepts Demonstrated

- User provisioning
- Security groups and group membership
- Least privilege
- Joiner-Mover-Leaver (JML) lifecycle
- Account deactivation
- Offboarding verification

## 6. Key Finding

Disabling a user account does not automatically remove that user from every group. During offboarding, administrators should separately review group memberships, application assignments, privileged roles, and active sessions according to organizational policy.

## 7. Test Results

The lab successfully demonstrated test-user creation, security-group membership, account deactivation, and post-deactivation group-membership verification.

Detailed test cases are documented in `test-cases.md`, and observations and recommendations are in `audit-findings.md`.

## 8. Limitations

- This is a small manual learning lab, not an automated audit solution.
- No Microsoft Graph or PowerShell automation was implemented.
- Group membership was demonstrated, but no application access was configured through the group.
- The lab does not claim to validate Conditional Access, MFA enforcement, or production security controls.

## 9. Future Improvements

- Automate user and group reporting with Microsoft Graph PowerShell.
- Detect enabled accounts that require offboarding review.
- Export findings to CSV.

- ## 10. Screenshots
- Entra ID Dashboard
Test User Accounts
IAM Security Group Membership
Account Deactivation
Group Membership After Deactivation
- Review application assignments and privileged role assignments.
- Add repeatable audit checks.


