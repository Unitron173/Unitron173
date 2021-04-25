# SSH Assignment-1
**Level 0**
~ssh bandit0@bandit.labs.overthewire.org -p 2220
~cat readme
***Learnt 'cat' command***
-------------------------
**Level 1**
~ssh bandit1@bandit.labs.overthewire.org -p 2220
~cat ./-
***Learnt to read data from conflicting filenames***

--------------------
**Level 2**
~ssh bandit2@bandit.labs.overthewire.org -p 2220
~cat 'spaces in this filename'
---------------------
**Level 3**
~ssh bandit3@bandit.labs.overthewire.org -p 2220
~ls
~cd inhere
~find
~cat ./.hidden
***Learnt to read data from hidden files***
------------------
**Level 4**
~ssh bandit4@bandit.labs.overthewire.org -p 2220
~ls
~cd inhere
~ls
~file ./-file*
~cat ./-file07
***Learnt to search for files with human readable data***
-----------------
**Level 5**
~ssh bandit5@bandit.labs.overthewire.org -p 2220
~ls
~cd inhere
~ls
~find -type f -size 1033c ! -executable
~cd maybehere07
~cat ./.file2
***Learnt to search for files with a particular size***
------------------
**Level 6**
~ssh bandit6@bandit.labs.overthewire.org -p 2220
~find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
~cat /var/lib/dpkg/info/bandit7.password
***Learnt to search for files used and grouped by different users***
-------------------
**Level 7**
~ssh bandit7@bandit.labs.overthewire.org -p 2220
~ls
~cat data.txt | grep millionth
***Learnt to search for text adjacent to a particular word***
---------------
**Level 8**
~ssh bandit8@bandit.labs.overthewire.org -p 2220
~ls
~sort data.txt | uniq -u
***Learnt to search for unique data in file***
--------------
**Level 9**
~ssh bandit9@bandit.labs.overthewire.org -p 2220
~cat data.txt | strings
~cat data.txt | strings | grep =
---------
**Level 10**
~ssh bandit10@bandit.labs.overthewire.org -p 2220
~cat data.txt | base64
~cat data.txt | base64 --decode
***Learnt to decode encoded data from txt file***
------
**Level 11**
~ssh bandit11@bandit.labs.overthewire.org -p 2220
~ls
~cat data.txt | strings
~cat data.txt | tr "[n-za-mN-ZA-M]" "[a-zA-Z]"
***Learnt how to use 'tr' command and how to decode ROT* cyphers***
------------
**Level 12**
~mkdir /tmp/darkstar48
~cp data.txt /tmp/darkstar48
~cd /tmp/darkstar48
~file data.txt
~xxd -r data.txt > data
~file data
~mv data data.gz
~gunzip data.gz
~file data
~mv data data.bz2
~bzip2 -d data.bz2
~ls
~file data
~mv data data.gz
~gunzip data.gz
~ls
~file data
~mv data data.tar
~tar -xf data.tar
~ls
~file data5.bin
~mv data5.bin data5.tar
~tar -xf data5.tar
~ls
~file data6.bin
~mv data6.bin data6.bz2
~bzip2 -d data6.bz2
~ls
~file data6
~mv data6 data6.tar
~tar -xf data6.tar
~ls
~file data8.bin
~mv data8.bin data8.gz
~gunzip data8.gz
~ls
~file data8
~cat data8

***Learnt how to decode a Hexdump using 'xxd', how to unzip bzip2, gzip and tar files and how to use the 'mv' command to rename files.***
----------
**Level 13**
~ls
~ssh -i sshkey.private bandit14@localhost
~yes
~cd /etc/bandit_pass
~ls
~cat bandit1

***Learnt how to use SSH keys to connect.***
-------------------
**Level 14**
~nc localhost 30000
~4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
>This is the password for bandit14 which we are asked to forward to port 30000 on localhost.

***Learnt how to use Netcat ('nc')***
----------------------
**Level 15**
~openssl s_client -connect localhost:30001
~BfMYroe26WYalil77FoDi9qh59eK5xNr
>This is the password for bandit15.

***Learnt how to use openssl's s_client command to send data with SSL encryption.***
-----------------
**Level 16**
