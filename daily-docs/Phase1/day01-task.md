
# Day 01 – AWS CLI Setup & IAM User Management

**Date:** 2025-10-07
**Objective:** Configure AWS CLI and create IAM users/groups.

---

## ✅ Commands Executed
```bash
aws configure
aws iam create-user --user-name devuser
aws iam create-group --group-name devteam
aws iam add-user-to-group --user-name devuser --group-name devteam
aws iam attach-user-policy --user-name devuser --policy-arn arn:aws:iam::aws:policy/ReadOnlyAccess
aws sts get-caller-identity


## 🤖 AI Prompt Practice
> "ChatGPT, generate a JSON IAM policy that grants S3 read-only and CloudWatch read-only permissions using least privilege.”

## 🧾 Notes / Learnings

Created IAM user devuser and group devteam.

Attached least-privilege ReadOnlyAccess policy.

Verified credentials using aws sts get-caller-identity.

Learned to manage IAM users, groups, and policies via CLI.

## 📸 Screenshots / Output
- [Optional]

## ✅ Checklist
 AWS CLI configured

 IAM user and group created

 Policy attached

 Verified IAM credentials


---

### **How to commit and follow progress for Day 1**
1. Save this file as `Day01_AWS_CLI_IAM.md` in your **Phase 1** GitHub folder.
2. Open terminal in the repo and run:
```bash
git add Phase1/Day01_AWS_CLI_IAM.md
git commit -m "Completed Day 1: AWS CLI setup and IAM user/group creation"
git push origin main
- [ ✅ ] Task completed