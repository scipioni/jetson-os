
# jetson os 

- https://www.forecr.io/blogs/installation/jetpack-5-1-installation-for-dsboard-ornx


- Jetson Orin NX: P3767-0000
- Jetson Xavier NX reference carrier board: P3509-0000 


## prereq

virtual machine with ubuntu 20.04 server

```
sudo snap install task --classic

```


## sdkmanager
s

download sdkmanager_1.9.2-10884_amd64.deb and install
```
sudo dpkg -i /tmp/sdkmanager_1.9.2-10884_amd64.deb
sudo apt -f install
```

show args
```
task show-args
```

download files
```
task download
```



