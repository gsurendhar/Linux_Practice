SSH key related commands


To generate SSH key from your system 

```
ssh-keygen -f <file-name>
```
To login to any linux server using Public-key and Private-key for this, before creating server you need to put your public-key in server by import key-pair option in AWS, then login using below command.

```
ssh -i <private-key> user-name@ip address
```

ssh login using password 

```
ssh user@ip address  
```

to print the System Information
```
uname
```
to print the all System Information
```
uname -a
```
present working directory
```
pwd
```
to change one directory to another directory use **cd** command
```
cd <path-where-to-go>
```
to list the content in that directory by **ls**
```
ls <options>
```
major options are
--> ```ls -l```     ----> to long listing format.
--> ```ls -a```     ----> to hidden files and folders.
--> ```ls -la```    ----> to long listing with hidden files.
--> ```ls -lr```    ----> to long listing with reverse alphabetic order.
--> ```ls -lt```    ----> to long listing with latest files on top.
--> ```ls -lh```    ----> to long listing with human readable format.
--> ```ls -ltr```   ----> to long listing with latest at bottom.
--> ```ls -lrth```  ----> to long listing with latest at bottom with human readable format.

