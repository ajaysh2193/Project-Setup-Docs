# Project-Setup-Docs

### command to connect to Mysql through terminal - 
mysql -h dwhdb.host.com -u username -P portno -p dbname

### command to connect to Redshift- 
psql -h  -U  -d dwh -p

### Copy Folder from local to server (for file, remove -r)

scp -i ~/Desktop/id_rsa.pub -P 9018 -r /home/ajay/filename ajay-sharma@proxy.server.com:/home/ajay-sharma/

### Login into server using ssh
ssh ajay-sharma@proxy.serverhost.com -p 9018

### Save db credentials used in code into .profile to avoid credentials in source code
- vi .profile
- export SR_Redshift_Host=redshift.kartrocket.com
- export SR_Redshift_Port=3315
- export SR_Redshift_User=ajay_sharma
- export PGPASSWORD=H8Fa2f9wAzGXTgQs
 - Entet "source .profile" into terminal

### Push project in git

- On local

1) cd Desktop

2) mkdir Kraftly

3) cd kraftly
4) git init

5) git remote add origin “Fork repo link”

6) git remote add upstream “Original repo link”

7) git fetch upstream master

8) git status

9) git pull upstream master

10) git status


- Same step on server from 1 to 10


11) Then again go to local system, copy your project to the created directory
12) git add file/folder
13) git commit -m “message”
14) git push origin master/other branch


- To update project in main repository
1) Create pull request from fork repo
2) Create merge request and submit it.
 
 
 
