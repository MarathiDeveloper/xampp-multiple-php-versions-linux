# xampp-multiple-php-versions-linux install

https://www.apachefriends.org/download.html

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

## Set environment variable PHP
```bash
        cd ~

        sudo gedit .bashrc
     //.bashrc file last add line 
     export PATH="/opt/lampp/bin:$PATH"
     export PATH="$HOME/.config/composer/vendor/bin:$PATH"
     
     source ~/.bashrc
