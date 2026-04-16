# Linux Lab #1 💻

## Scenario:
In response to heightened security concerns, the xFusionCorp Industries security team has implemented custom Apache users for their web applications. Each user is tailored to a specific application to enhance security.

## Task:
a. Create a user named john in the local Linux system.\
b. Assign a unique UID (1888) and set the home directory to /var/www/john.

## Solution:

```bash
sudo useradd -u 1888 -d /var/www/john -m john
```

## Verification:

```bash
id john
ls -ld /var/www/john
```
