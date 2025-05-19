# Package Management commands
In linux there are many distributions in that major are RHEL(AlmaLinux, Rocky Linux, ClearOS, Oracle Linux and CentOS) and Debian(Ubuntu, Kali Linux and Linux Mint)

In this RHEL and Debian some Package Management commands are different.

In RHEL `yum` or `dnf` command is used.
```
yum install <package-name>
```
```
dnf install <package-name>
```
But in Debian `apt` or `apt-get` is used.

```
apt install <package-name>
```
```
apt-get install <package-name>
```
**RHEL**
```
dnf install <package-name> <options>
```
`-y` ---> is used to install directly instead of asking do you want install or not

ex:- `dnf install python -y`

To list out the installed packages by
```
dnf list installed
```
To remove/uninstall the installed package by 
```
dnf remove <package-name>
```
ex:- `dnf remove python -y`

To list out available packages in repo

```
dnf list available
```

All available packages are there in directory is 

```
/etc/yum.repos.d
```

**If there is any package is not available in a repo, we need to add the repo of that package and that repo file extension should be `.repo`.**
ex:- `vim /etc/yum.repos.d/mongodb-org-8.0.repo`

then add the installation configuration file from official web-site

```
[mongodb-org-8.0]
name=MongoDB Repository
baseurl=https://repo.mongodb.org/yum/redhat/8/mongodb-org/8.0/x86_64/
gpgcheck=1
enabled=1
gpgkey=https://pgp.mongodb.com/server-8.0.asc
```

then install package by `dnf` command
```
dnf install mongodb-org -y
```

we can also enable and disable particular version of package available in repo
```
dnf module disable nginx -y
```
```
dnf module enable nginx:1.24 -y
```
then
```
dnf install nginx -y
```
