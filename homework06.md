<h1>a)</h1>
To install Hashcat I used https://terokarvinen.com/2022/cracking-passwords-with-hashcat/ for instructions


<h6>1.</h6>
First I had to install the apps with these commands:

$ sudo apt-get update
$ sudo apt-get -y install hashid hashcat wget

<h6>2.</h6>
then I had to make a new directory. 

$ mkdir hashed
$ cd hashed

<img width="409" alt="image" src="https://github.com/user-attachments/assets/c7038dc8-bc86-420b-b3b0-644ef224bec0">





<h6>3.</h6>

We need dictionary since we want our computer to try to find match for our hash. So I downloaded the dictionary. I used Rockyou.

$ wget https://github.com/danielmiessler/SecLists/raw/master/Passwords/Leaked-Databases/rockyou.txt.tar.gz
$ tar xf rockyou.txt.tar.gz
$ rm rockyou.txt.tar.gz


<h6>4.</h6>
Then to identify the hash type I used

$ hashid -m 6b1628b016dff46e6fa35684be6acc96

The hash is an example. To identify whichever hash you would like, replace it. 
After we wrote this command we get info about the hash.

<h6>5.</h6>
So now that we have info I chose the second one MD5 that had "0" as parameter, since it's very common and it was second on three candidates.
Now it was time to crack the hash, using command:

$ hashcat -m 0 '6b1628b016dff46e6fa35684be6acc96' rockyou.txt -o solved

$ cat solved 


Then we got the right password!







<h1>b)</h1>

To crack this hash I jsut used the same steps as in the a) exercise from 4-6, then I got it easily cracked!


<img width="389" alt="image" src="https://github.com/user-attachments/assets/0a7962ea-4e64-4f2a-bcac-2429f4bef8d0">





<img width="402" alt="image" src="https://github.com/user-attachments/assets/d05dea97-fcaa-4a84-ba39-a60e4819c619">





<img width="227" alt="image" src="https://github.com/user-attachments/assets/e1936dc9-fe29-403d-8945-9e251cca6287">



