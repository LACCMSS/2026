---
title: Accessing the HPC
---

# Accessing the LANL HPC



## MAC
To connect to Chicoma via ssh use:
```
>> ssh -I/usr/lib/ssh-keychain.dylib <moniker>@wtrw.lanl.gov
>> ssh ch-fe
```
or you can configure the "config" file inside the '.ssh' folder in you home directory with
```
Host wtrw.lanl.gov
  HostName wtrw.lanl.gov
  PKCS11Provider /usr/lib/ssh-keychain.dylib
  User <moniker>
```
then you can use 
```
>> ssh <moniker>@wtrw.lanl.gov
>> ch-fe
```
to log into chicoma.


## Linux

### Installing OpenSC 
To get the opensc-pkcs11.so library on your Linux system, you need to install the OpenSC package. Depending on your Linux distribution, the exact location of the file might vary slightly (such as /usr/lib/x86_64-linux-gnu/opensc-pkcs11.so or /usr/lib64/opensc-pkcs11.so), but installing the core package will provide it.
```
sudo apt update
sudo apt install opensc opensc-pkcs11
```

### Connecting to Chicoma
To connect to Chicoma via ssh use:
```
>> ssh -I/usr/lib/x86_64-linux-gnu/opensc-pkcs11.so <moniker>@wtrw.lanl.gov
>> ssh ch-fe
```
or you can configure the "config" file inside the '.ssh' folder in you home directory with
```
Host wtrw.lanl.gov
  HostName wtrw.lanl.gov
  PKCS11Provider /usr/lib/x86_64-linux-gnu/opensc-pkcs11.so
  User <moniker>
```
then you can use 
```
>> ssh <moniker>@wtrw.lanl.gov
>> ch-fe
```
to log into chicoma.


## Windows

### Install OpenSC
1. Download the latest stable version of OpenSC from its GitHub repo: [https://github.com/OpenSC/OpenSC](https://github.com/OpenSC/OpenSC). For 64-bit and 32-bit programs use OpenSC*_win64.msi and OpenSC*_win32.msi, respectively.
2. Run the installer as an admin. 
3. Then, with the card reader connected and the PiV/zToken card inserted, test the PKCS#11 support of your card with one of these options in cmd.exe (this should also work on PowerShell):
```
>> "C:\Program Files\OpenSC Project\OpenSC\tools\pkcs11-tool.exe" --login --test
>> "C:\Program Files (x86)\OpenSC Project\OpenSC\tools\pkcs11-tool.exe" --login –test
```
This should read the PiV/zToken and ask for your PiV/zToken Pin. 
4. After generating a certificate, you can try to SSH:
```
>> ssh -I “<installation path>\OpenSC Project\OpenSC\pkcs11\opensc-pkcs11.dll” <moniker>@wtrw.lanl.gov
```
5. If it works, your full name should be prompted, and you should be asked again for your PiV/zToken Pin.
6. After that, connect to Chicoma through:
```
>> ssh ch-fe
```
7. You can check the “config” file generated in the “.ssh” folder, which is typically inside your <username> folder. It should look something like this:
```
Host wtrw.lanl.gov
  HostName wtrw.lanl.gov
  PKCS11Provider "<installation path>\OpenSC Project\OpenSC\pkcs11\opensc-pkcs11.dll"
  User <moniker>
```
Note: if the file is not generated, you can create it and follow the previous structure.

8. If the config is ok, the following SSH commands will only need:
```
>> ssh <moniker>@wtrw.lanl.gov
```
Note: <installation path> should be “C:\Program Files\” or “C:\Program Files (86)\”

### Connecting to Chicoma
To connect to Chicoma via ssh use:
```
>> ssh -I “<installation path>\OpenSC Project\OpenSC\pkcs11\opensc-pkcs11.dll” <moniker>@wtrw.lanl.gov
>> ssh ch-fe
```
or if the ssh config file is set up
```
>> ssh <moniker>@wtrw.lanl.gov
>> ch-fe
```



