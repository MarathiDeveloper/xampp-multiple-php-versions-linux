# xampp-multiple-php-versions-linux install

https://www.apachefriends.org/download.html

## प्रथम [https://www.apachefriends.org/download.html](https://www.apachefriends.org/download.html) या वेबसाईटवर तुम्हांला जे PHP version पाहीजे ते डाउनलोड करा. 

```bash
cd Downloads/  
```
जा आणि त्या फाईल Permission दया. 

```bash

sudo chmod 755 xampp-linux-*-installer.run

sudo ./xampp-linux-*-installer.run

cd /opt 

```

वर जाऊन lampp या फोल्डरचे नाव change करा ते कोणतं PHP Version आहे हे कळण्यासाठी 

```bash

sudo  lampp  lampp7_4

 cd /opt
 sudo lampp7421/lampp stop
 sudo rm -r lampp

```
