# Solving-ExpoCli-android-error
The something went wrong and timeout error. 
Have you been coding in React Expo application and sometimes you encounter such a problem?. Here is how you can solve this problem.

![image](https://github.com/dennisngugiwambui/Solving-ExpoCli-android-error/assets/112067611/9f87d37e-551b-4f0e-90e9-ede8c0768d46)


Open powershell and run as administrator

```ipconfig```
You will see the following:
```
Wireless LAN adapter Wi-Fi:

   Connection-specific DNS Suffix  . : zuku.co.ke
   Link-local IPv6 Address . . . . . : fe80::7d9d:781e:5b0:4097%7
   IPv4 Address. . . . . . . . . . . : 192.168.0.16
   Subnet Mask . . . . . . . . . . . : 255.255.255.0
   Default Gateway . . . . . . . . . : 192.168.0.1
   ```
 Now from this select the ```IPv4 Address. . . . . . . . . . . : 192.168.0.16```
 now you can run the following command in the powershell:
 ```setx /M REACT_NATIVE_PACKAGER_HOSTNAME 192.168.0.16```
 Now close the terminal and then reopen the terminal again and run
 ```npm run android```
 
 This should now not return any error
