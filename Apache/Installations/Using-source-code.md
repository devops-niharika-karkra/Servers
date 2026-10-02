# Installing Apache Using Source Code
As we know Apache is Open source. So, one can install apache using soucre code also. Installing it with source code provide the precise control over modules and packages.

## What is Source code? 
  Source code is software written maily in programming languages such as C, C++, etc, to build packages like Apache.

## Why? 
  Because when we install package from source code, you work with the original code of apache and can even customise it according to your requirements.


### Step 1: Install Dependencies
These are tools and libraries required to build Apache.

For example:
  - build-essential → This installs the fundamental tools needed for compiling software in Linux.
  - libpcre2-dev → PCRE stands for Perl Compatible Regular Expressions.
  - libapr1-dev → APR stands for Apache Portable Runtime.
  - libapr1-dev → APR stands for Apache Portable Runtime. It is a core library that provides a predictable interface across different operating systems.
  - libaprutil1-dev → This is the APR Utility library. It extends the standard APR by providing Apache with higher-level developer tools
  - libssl-dev → This package provides the development headers for OpenSSL. 

command
```
  sudo apt update
  sudo apt install -y build-essential \
  libpcre2-dev \
  libapr1-dev \
  libaprutil1-dev \
  libssl-dev \
```

<img width="1165" height="221" alt="image" src="https://github.com/user-attachments/assets/5352fea5-bd94-4f78-9dab-5d292ec59045" />

Why?
Your Linux machine doesn't automatically have everything required to compile Apache. 

### Step2: Download Apache Source Code 
This installs Apache source code in archive form. This is the main file through which we will install Apache in our system.
```
  wget https://dlcdn.apache.org/httpd/httpd-2.4.69.tar.bz2
```
<img width="1151" height="325" alt="image" src="https://github.com/user-attachments/assets/6cd16892-500b-4240-bc18-24be418e27ff" />

### Step3: Extract the Source code 
In tis step, we will extract the files of archived source code. These are the actual files we need to install Apache.
```
  tar -xf httpd-2.4.68.tar.bz2
```
<img width="1148" height="88" alt="image" src="https://github.com/user-attachments/assets/afefb52f-f567-41f7-b12a-c76ca7398bab" />

### Step4: Make a directory
Make an empty directory in this we will install Apache. 
```
  mkdir apache2.4.68
```
<img width="1010" height="31" alt="image" src="https://github.com/user-attachments/assets/42d2b7ee-9b36-4f3e-99f0-e9a383924c87" />

### Step5: Change directory
Change directory to te folder which contains the files of source code. In this folder we have some executables such as configure and make which will help us to install the Apache.
```
  cd httpd-2.4.68
```
<img width="1010" height="31" alt="image" src="https://github.com/user-attachments/assets/971e34d5-e233-4bfb-96b8-7692b3abc2ff" />

### Step6: Configure Apache
This is used to configure the source code of Apache HTTP Server before compiling and installing it on a system.
```
  ./configure --prefix=/home/ubuntu/apache2.4.68 --enable-shared=max
```
  - --prefix: Defines the installation directory
  - --enable-shared: Tells the compiler to build as many Apache modules as possible as Dynamic Shared Objects.
    
<img width="1153" height="313" alt="image" src="https://github.com/user-attachments/assets/e40f23ad-69e7-46ed-872d-f27e83d114d0" />

### Step7: Compile and install Apache 
In this step, we will run command to compile and deploy software from its raw source code.
```
  make && make install
```
<img width="1152" height="301" alt="image" src="https://github.com/user-attachments/assets/0a6cc96f-3d25-4a5f-a635-008f7933f1af" />

### Step8: Change directory to Folder you created
```
  cd apache2.4.68
```
<img width="1132" height="30" alt="image" src="https://github.com/user-attachments/assets/d282b7d5-7158-4ad0-b3f8-78238d9b7c71" />

### Step9: Changes in apache's configuration
Open httpd.conf from conf directory and change the port from 80 to 8080. As we are working as ubuntu user and don't have permissions to run any service without sudo on port numbers less than 1024. 
If you'll try to start apache using sudo then you'll get permission errors.
NOTE: You can even perform all these steps through root user and then you won't be required to change the port number
```
  vim conf/httpd.conf
```
<img width="1132" height="30" alt="image" src="https://github.com/user-attachments/assets/22ee3e56-a0cb-4dbb-9e22-665d0255773b" />

### Step10: Change the port number
<img width="832" height="303" alt="image" src="https://github.com/user-attachments/assets/d5ac335a-5e61-4d2a-a8a0-562b5f99f425" />

### Step11: Start Apache
```
  /home/ubuntu/apache2.4.68/bin/apachectl start
```
<img width="1132" height="30" alt="image" src="https://github.com/user-attachments/assets/ca662565-e83d-42dd-a05e-449678b3b0c0" />

### Step12: Verify whether it is running or not
#### To check the service it running you can do three things
```
  curl localhost:8080
```
<img width="1133" height="285" alt="image" src="https://github.com/user-attachments/assets/8917c280-ff2e-47ec-8d3e-e8f2ff9e4eb7" />


#### You can run command to check in processes and grep the folder name in which your apache was installed
```
  ps -ef | grep 'apache'
```
<img width="1198" height="198" alt="image" src="https://github.com/user-attachments/assets/80e88d13-a106-47b1-9229-8067f09d5a11" />

#### You can paste your public ip with the port number 
```
  http://<ip>:8080
```
<img width="632" height="258" alt="image" src="https://github.com/user-attachments/assets/3afef054-cc47-48d7-b076-3e139d640788" />



