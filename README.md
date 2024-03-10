# Hive, Cortex and MISP Integration Guide

This guide will walk you through setting up Hive, Cortex and MISP Integration.
## Prerequisites:
Installed docker and docker compose

## Commands to run:
i.  first up(install):
    docker compose up -d
ii. remove all containers:
    docker compose down
iii. start a previous compose:
    docker compose start
iv. stop a previous compose:
    docker compose stop

## Caution 
You may need to increase vm.max_map_count.To do this:
We need to add below line in /etc/sysctl.conf file and then run sysctl -p to apply the changes.
vm.max_map_count = 1048575

## Cortex API key
Firstly, Go to "Add organization".
![image](https://github.com/Nahin009/pyMisp/blob/Hive%26Cortex%26MISP-Integration/images/Cortex/0.png)

then input necessary information and save.
![image](https://github.com/Nahin009/pyMisp/blob/Hive%26Cortex%26MISP-Integration/images/Cortex/1.png)

then click "Add user" button and input necessary information with orgadmin role
![image](https://github.com/Nahin009/pyMisp/blob/Hive%26Cortex%26MISP-Integration/images/Cortex/2.png)

then click Reveal to get the API key
![image](https://github.com/Nahin009/pyMisp/blob/Hive%26Cortex%26MISP-Integration/images/Cortex/3.png)

then copy the key
![image](https://github.com/Nahin009/pyMisp/blob/Hive%26Cortex%26MISP-Integration/images/Cortex/4.png)



## Creating `.env` File

In the main directory of your project, create a file named `.env`. This file will store sensitive information securely. Add the following line to the `.env` file:

```plaintext
MISP_API_KEY="your misp api key"
```

## run the code

Copy-Paste all the commands in the "commands" file in the terminal and click enter 
