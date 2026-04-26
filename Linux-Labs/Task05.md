# 🐧 Linux Lab #5

## Scenario:

Following security audits, the xFusionCorp Industries security team has rolled out new protocols, including the restriction of direct root SSH login.

---

## Task:

Your task is to disable direct SSH root login on all app servers within the Stratos Datacenter.

<img width="1152" height="257" alt="image" src="https://github.com/user-attachments/assets/d8fdf29d-9f8d-4e71-8bed-d35e840516e2" />


---

## Solution: 
To disable direct root SSH login on all your app servers, you’ll need to update the SSH configuration on each server and restart the SSH service.

**Run on each app server:**

```
ssh tony@stapp01
password for tony

# Open SSH config file
sudo vi /etc/ssh/sshd_config

# Find this line:
PermitRootLogin yes

# Change it to:
PermitRootLogin no

# If the line doesn’t exist, just add it manually.
# Save and exit

# Restart SSH service
sudo systemctl restart sshd

# or
sudo systemctl restart ssh
```

---

## ✅ Verification

**Try logging in as root:**

```
ssh root@<server-ip>
```

**Permission denied!**

---
