
----------------Task Number 1 -----------------------------------------------------------------
Q1) 
- Installed 

Q2)
Cat --> we use to show all the file at the time it suitable for smallfile
more --> it suitable to large file which it show the file page by page

Q3)
rm --> to remove files and we can use to remove Dir by using other command with it 
rmdir -->  to remove empty dir 

Q4)
- mkdir -p ~/dir1/dir11
- mkdir -p ~/dir1/dir12
- mkdir -p ~/docs/mycv
- touch  ~/dir1/dir12/file 
rmdir ~/dir1/dir11 --> can not remove becaus it is empty 
rm -r ~/dir1/dir11 --> it removed 
rmdir -p ~/dir1/dir12 --> dir not empty 
- cd docs , cd mycv , pwd 

Q5)
- cp /etc/passwd  ~/mypasswd  

Q6) 
- mv ~/mypasswd  ~/oldpasswd

Q7)
-CD
-CD ~
-CD $home

Q8)
- ls user/bin/w* 
- sudo ls user/bin/w*

Q9) 
- head -n 4 /etc/passwd

Q10)
- tail -7 /etc/passwd

Q11)
-man passwd && man 5 passwd 

Q12)
- man 5 passwd

Q13)
- man -k passwd 

Q14) 
- vi mycv  -- > i to input , :wq --> to save , q --> to exist 

Q15)
- vi mycv --> j,k --> up and down ,, h,l --> right and left ,, /age --> to search about age ,, 
5g --> move to line num 5 ,, :5d --> delete the 5 line ,, dd --> delete the next line 


Q16)
- cat /etc/shells 

-----------------------------------------------task 2 --------------------------------------------------------------
cat /etc/shells                          Q1

printenv                                Q2

echo $SHELL                              Q3

env                                     Q4

echo "Welcome! Today is $(date)" >> ~/.bashrc         Q5

echo 'export PS1="[\u@\h \W]$ "' >> ~/.bashrc          Q5

ls > file_list.txt                      Q6

ls *.txt                                Q7

ls >> file_list.txt                     Q8

ls | grep report                         Q9

head filename.txt                        Q10

tail filename.txt                        Q10

cut -d',' -f2 data.csv                  Q11

grep "ERROR" log.txt                     Q12

current_user=$(whoami)                  Q13

echo "hello world" | tr 'a-z' 'A-Z'      Q14

ps aux | grep process_name               Q15

alias ls='ls -l'                        Q16

ls -lS                                  Q17

grep -c "success" filename.txt           Q18

dmesg > dmesg_output.txt                Q19

head -n 20 dmesg_output.txt             Q19

cut -d',' -f1 filename.csv              Q20


----------------------task 3-------------------------
Q1 )
-sudo useradd muhammed -m  -c 'muhammed qadri'
- sudo passwd muhammed 

Q2)
-sudo useradd baduser -m -c 'baduser'
-sudo paswwd baduser

Q3)
- groupadd -g 30000 pgroup 

Q4)
- sudo groupadd -g 20000 badgroup

Q5)
- sudo usermod -g pgroup muhammed 
- groups muhammed --> to retrive muhammed group

Q6)
- sudo passwd muhammed 

Q7)
-sudo chage -m 30 muhammed

Q8)
- sudo passwd -l baduser --> to lock password or sudo chage E0 baduser --> to expired or usermod -e1 baduser --> to block account
- sudo passwd -u baduser --> unlock

Q9)
-sudo passwd -d baduser

Q10)
- sudo groupdel badgroup 

Q11)
- chmod myteam r

Q12)
- sudo su 'muhammed'

Q13)
- CD myteam 

Q14)
- sudo chmod u=rw,g=rx,o=x oldpasswd
- sudo chmod u=rwx,g=rwx,o=rwx oldpasswd
- sudo setfacl -PRdm u::rwx,g::rwz,o::rwx --> to put default permission to all file

Q15) 
- find /home/ -mtime -2 -ls

Q16)
- find /etc -user root --> to find all user owned by root 

Q17)
- sudo find ~ -type d --> to return all dirctories in home 

Q18
- sudo find / -type f -name profile

Q19)
- file /etc/passwd 
- file /dev/pts/0 
- file /etc
- file /dev/sda

Q20)
- ls -i /
- ls -i /etc
- ls -i /etc/hosts

Q21)
-cp /etc/passwd ~/
-diff /etc/passwd ~/passwd
-cmp /etc/passwd ~/passwd
-nano ~/passwd
-diff /etc/passwd ~/passwd
-cmp /etc/passwd ~/passwd

Q22)
-sudo ln -s /etc/passwd /boot/passwd  --> to create softlink

Q23)
- u can not make hard link must be in the same palce

-------------------------------Task 4 -------------------------------------------
Q1)
- ps aux > ~/process.txt
 
Q2)
- ps -ax | grep sshd or ps -elf | grep sshd

Q3)
- sleep 500
- sleep 5
- ps --> to get parent id 
- kill -9 6680

Q4)
-sudo apt update
-sudo apt install -apache2 -y
-sudo nano /var/www/html/index.html

Q5)
-sudo apt install openssh-server -y(install sshd)
-sudo systemctl status ssh
-sudo systemctl start ssh 

Q6)
- sudo systemctl status cron 
- sudo systemctl start cron 

Q7)
-sudo tar -czvf archive.tar.gz /var/log   --> to create archieve file contain all file in dir /var/log

Q8)
- mkdir ~/logs-bakup/
-tar -xzf archive.tar.gz -C ~/logs_bakup/

Q9)
-sudo tar -cvf /tmp/archive.tar /etc/ssh

Q10)
-gzip ~/process.txt 

Q11)
-gunzip ~/process.txt.gz
-cp  ~/process.txt.gz  ~/process_copy.txt.gz
-ls -lh ~/process_copy.txt.gz ~/processes.txt.gz

Q12)
- sudo apt update 
- sudo apt install htop -y

Q13
- apt search nginx
- apt search httpd

Q14
-sudo apt remove --purge vim -y
- sudo apt install vim -y

Q15)
-wget https://cdn.kernel.org/pub/linux/kernel/v6.x/linux-6.1.tar.xz

Q16)
-curl https://www.google.com -o google.html

Q17)
- sudo adduser Ali
-sudo usermod -aG sudo ali







