## Install ubuntu-linux-on-wsl

```bash
apt install libssl-dev -y -q
apt autoremove libfreetype6 -y -q 
apt update -y -q
```


```bat
ubuntu config --default-user root
```

```bat
ubuntu config --default-user <username>
```

## list-users
The /etc/passwd file is a colon-separated file that contains the following information:
* User name
* Encrypted password
* User ID number (UID)
* User's group ID number (GID)
* Full name of the user (GECOS)
* User home directory
* Login shell

```bash
less /etc/passwd
```

## list-users - when the number of users is small

```bash
cat /etc/passwd
```
## change-password
```bash
passwd <username>
```
