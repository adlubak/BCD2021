## 1. Utworzenie pary kluczy
*$ ssh-keygen -t rsa*

**Output:**

Generating public/private rsa key pair.  
Enter file in which to save the key (/home/piotr/.ssh/id_rsa):   
Enter passphrase (empty for no passphrase):   
Enter same passphrase again:   
Your identification has been saved in /home/piotr/.ssh/id_rsa  
Your public key has been saved in /home/piotr/.ssh/id_rsa.pub  
The key fingerprint is:  
SHA256:R72P/HBjn48IDXmEGJ6URF4DaoQOucYqBadR3avojBw piotr@15  
The key's randomart image is:  
+---[RSA 3072]----+  
| ..o o.o*oo      |  
|o + o..=.= +     |  
| * +  o.= o o    |  
|. = ...  . o .   |  
| + . .  S + o    |  
|oE. .    . = o   |  
|o+.       . = =  |  
|..o        . * +.|  
|            . o.+|  
+----[SHA256]-----+  


## 2. Skopiowanie klucza publicznego do maszyny wirtualnej
**Sposoby:**  
a) użycie polecenia *ssh-copy-id*  
b) skopiowanie zawartości klucza publicznego *id_rsa.pub* do *~/.ssh/authorized_keys*  

**Próba logowania:**

*$ ssh ubuntu@156.17.252.232 -p 40044*

Welcome to Ubuntu 18.04.1 LTS (GNU/Linux 4.15.0-161-generic x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage ...

