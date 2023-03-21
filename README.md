
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

download sdkmanager_1.9.2-10884_amd64.deb in /tmp and install
```
sudo dpkg -i /tmp/sdkmanager_1.9.2-10884_amd64.deb
sudo apt -f install
```

login to nvidia devzone
```
task login
```

download JetPack 5.1 (rev. 1) Linux for Jetson AGX Orin modules files into ~/Downloads/nvidia/sdkm_downloads/
```
task download
```

build image
```
task build
```



