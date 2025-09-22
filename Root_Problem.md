Problem 1
---

You can't install software. when you try to install a package on the terminal, is says:
```bash
user is not in the sudoers file.
```
*I got you!*

Step 1
---
Run:
```bash
su -
usermod -aG sudo $USER
exit
```
and then restart your computer.

---
To check if it worked, type:
```bash
sudo whoami
```
it should say:
```bash
root
```
---

Problem solved!


When you can't install anything, you don't have root.
root is the thing that gives you administrator rights.
