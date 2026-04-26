# 🐧 Linux Lab #4

## Scenario:

In response to the latest tool implementation at xFusionCorp Industries, the system admins require the creation of a service user account. Here are the specifics:

## Task:

Create a user named ravi in App Server 3 without a home directory.

<img width="1186" height="389" alt="image" src="https://github.com/user-attachments/assets/5138e6ca-9992-4edc-a705-918e02f2d8be" />

## Solution:

```
ssh banner@stapp03
password of banner:
id ravi
sudo useradd -M ravi
password of banner:
id ravi
getent passwd ravi
```
