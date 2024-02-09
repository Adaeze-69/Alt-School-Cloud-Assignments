# Linux Exercise:
> Your login name: altschool i.e., home directory /home/altschool. The home directory contains the following sub-directories: code, tests, personal, misc Unless otherwise specified, you are running commands from the home directory.

---


>i. create login name called Altschool

![log in user](./Images/Log%20in%20user.PNG)

 >ii. Switch user from Adaeze to Altschool user created

 ```
 sudo su Altschool
 ```

 ![sWitch user](./Images/switch%20user%20to%20Altschool.PNG)

 >iii.  create sub directories  named code tests personal misc

 ```
mkdir code tests personal misc
```
![Create user](./Images/Create%20directories.PNG)

 
---

## Instructions
> a.Change directory to the tests directory using absolute pathname

```
cd /home/Altschool/tests
```
![absolute pathname](./Images/a.PNG)

---

>b. Change directory to the tests directory using relative pathname

```
cd ./tests
```
![relative pathname](./Images/b.PNG)

---

>c. Use echo command to create a file named fileA with text content ‘Hello A’ in the misc directory

```
echo 'Hello A' > misc/fileA
```
![echo command](./Images/c.PNG)

---
>d. Create an empty file named fileB in the misc directory. Populate the file with a dummy content afterwards

```
touch misc/fileB
```

```
nano misc/fileB
```
```
cat misc/fileB
```
![create an empty file](./Images/d.PNG)

---

>e. Copy contents of fileA into fileC

```
cp misc/fileA misc/fileC
```
![copy contents](./Images/e.PNG)

---
>f. Move contents of fileB into fileD

```
mv misc/fileB misc/fileD
```
![move contents](./Images/f.PNG)

---

>g. Create a tar archive called misc.tar for the contents of misc directory

```
tar -cvf misc.tar misc
```
![create misc.tar](./Images/g.PNG)

---

>h. Compress the tar archive to create a misc.tar.gz file

```
gzip misc.tar
```
![compress archived file](./Images/h.PNG)

---

>i. Create a user and force the user to change his/her password upon login

```
sudo chage -d 0 praise
```
![force user to change password](./Images/i.PNG)

---

>j.Lock a users password

```
sudo passwd -l praise
```
![lock user password](./Images/j.PNG)

---

>k. Create a user with no login shell 

```
sudo useradd -s /sbin/nologin Vicky
```
![no login shell](./Images/k.PNG)

---

>l. Disable password based authentication for ssh

```
 sudo vi /etc/ssh/sshd_config
```
![diasable password auth for ssh](./Images/l.PNG)

---

>m. Disable root login for ssh

```
vi /etc/ssh/sshd_config
```
![disable root login for ssh](./Images/m.PNG)