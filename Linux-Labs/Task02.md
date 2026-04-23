# Linux Lab #2 💻

To accommodate the backup agent tool's specifications, the system admin team at xFusionCorp Industries requires the creation of a user with a non-interactive shell. Here's your task:

## Scenario:
Create a user named mark with a non-interactive shell on App Server 1.


##  Details of Server 1:

<img width="1110" height="217" alt="image" src="https://github.com/user-attachments/assets/cc76491f-ef4b-471a-8fd5-f6a98f9e5543" />

-----

## Solution:

```
ssh tony@stapp01
password: 
```

**Become a Root user**

```
sudo su
OR
sudo -i #interactive shell
```

**Add user mark with no shell**
```
useradd -s /sbin/nologin mark
```

**Verify:**
```
getent passwd | grep mark
```


