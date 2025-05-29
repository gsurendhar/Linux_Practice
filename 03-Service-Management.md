To start the service by below command
```
systemctl start <Service-name>
```
To stop the service by below command

```
systemctl stop <Service-name>
```
Check the status of the service

```
systemctl status <Service-name>
```
To Enabling the service (enabling means auto start when system restarted or shutdown)
```
systemctl enable <Service-name>
```
To Disabling the service (disabling the auto restart)

```
systemctl disable <Service-name>
```
This all service files are there in `/etc/systemd/system/` this directory with a file extension of `.service` 
