# xampp multiple php versions linux install
## xampp start stop & php versions switch commands

## [https://www.apachefriends.org/download.html](https://www.apachefriends.org/download.html) या वेबसाईटवर तुम्हांला जे PHP version पाहीजे ते डाउनलोड करा. 

```bash
cd Downloads/  
```
xampp डाउनलोड केलेल्या file ला Permission दया. 

```bash

sudo chmod 755 xampp-linux-*-installer.run

sudo ./xampp-linux-*-installer.run

cd /opt 

```

वर जाऊन lampp या फोल्डरचे नाव change करा ते कोणतं PHP Version आहे हे कळण्यासाठी 
 
```bash

  sudo mv lampp lampp7_4

```
### Xampp Run Commands  

```bash
 cd /opt
 sudo ln -s lampp7_4/ lampp
 sudo lampp7421/lampp start
 
```
### Xampp Stop Commands  
```bash
  sudo lampp7_4/lampp stop
  sudo rm -r lampp
```
### install Composer [https://getcomposer.org/download/](https://getcomposer.org/download/) 
```bash
  php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
  
  php -r "if (hash_file('sha384', 'composer-setup.php') === '55ce33d7678c5a611085589f1f3ddf8b3c52d662cd01d4ba75c0ee0459970c2200a51f492d557530c71c15d8dba01eae') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
  
  php composer-setup.php
 
  php -r "unlink('composer-setup.php');"
 
  sudo mv composer.phar /usr/local/bin/composer
```

## Set global environment variable PHP
```bash
        cd ~

        sudo gedit .bashrc
```

## .bashrc file मध्ये शेवटी दोन line Add करा.
 
``` bash

     export PATH="/opt/lampp/bin:$PATH"
     export PATH="$HOME/.config/composer/vendor/bin:$PATH"
```
##  Save केल्यानंतर command Run करा.
```bash 
   source ~/.bashrc
```   
