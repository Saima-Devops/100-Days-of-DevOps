# 🐧 Linux Lab #3 

## Scenario:

As part of the temporary assignment to the Nautilus project, a developer named john requires access for a limited duration. 
To ensure smooth access management, a temporary user account with an expiry date is needed. Here's what you need to do:

## Task:

- Create a user named john on App Server 2 in Stratos Datacenter. 
- Set the expiry date to 2026-12-07, ensuring the user is created in lowercase as per standard protocol.

<img width="1159" height="266" alt="image" src="https://github.com/user-attachments/assets/b633756d-7c7f-4995-b45e-e6b063cf827c" />


## Solution:

```
ssh steve@stapp02
password: 
```

Check if john is already there

```
cat etc/passwd | grep john
```
john is not there so let's add him

```
sudo useradd john
sudo chage -l john
sudo usermod -e 2026-12-07 john
sudo chage -l john
```
