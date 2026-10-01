# Installing Apache Using Source Code
As we know Apache is Open source. So, one can install apache using soucre code also. Installing it with source code provide the precise control over modules and packages.

## What is Source code? 
  Source code is software written maily in programming languages such as C, C++, etc, to build packages like Apache.

## Why? 
  Because when we install package from source code, you work with the original code of apache and can even customise it according to your requirements.


### Step 1: Install Dependencies
These are tools and libraries required to build Apache.

For example:
build-essential → This installs the fundamental tools needed for compiling software in Linux.
libpcre2-dev → PCRE stands for Perl Compatible Regular Expressions.
libapr1-dev → APR stands for Apache Portable Runtime.
libapr1-dev → APR stands for Apache Portable Runtime. It is a core library that provides a predictable interface across different operating systems.
libaprutil1-dev → This is the APR Utility library. It extends the standard APR by providing Apache with higher-level developer tools
libssl-dev → This package provides the development headers for OpenSSL. 

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

wget
<img width="1151" height="325" alt="image" src="https://github.com/user-attachments/assets/6cd16892-500b-4240-bc18-24be418e27ff" />

tar
<img width="1148" height="88" alt="image" src="https://github.com/user-attachments/assets/afefb52f-f567-41f7-b12a-c76ca7398bab" />

mkdir
<img width="1010" height="31" alt="image" src="https://github.com/user-attachments/assets/42d2b7ee-9b36-4f3e-99f0-e9a383924c87" />

cd
<img width="1010" height="31" alt="image" src="https://github.com/user-attachments/assets/971e34d5-e233-4bfb-96b8-7692b3abc2ff" />

configure
<img width="1153" height="313" alt="image" src="https://github.com/user-attachments/assets/e40f23ad-69e7-46ed-872d-f27e83d114d0" />

make 
<img width="1152" height="301" alt="image" src="https://github.com/user-attachments/assets/0a6cc96f-3d25-4a5f-a635-008f7933f1af" />

cd to apache
<img width="1132" height="30" alt="image" src="https://github.com/user-attachments/assets/d282b7d5-7158-4ad0-b3f8-78238d9b7c71" />

changes
<img width="1132" height="30" alt="image" src="https://github.com/user-attachments/assets/22ee3e56-a0cb-4dbb-9e22-665d0255773b" />

start 
<img width="1132" height="30" alt="image" src="https://github.com/user-attachments/assets/ca662565-e83d-42dd-a05e-449678b3b0c0" />

verify
<img width="1133" height="285" alt="image" src="https://github.com/user-attachments/assets/8917c280-ff2e-47ec-8d3e-e8f2ff9e4eb7" />
or
<img width="632" height="258" alt="image" src="https://github.com/user-attachments/assets/3afef054-cc47-48d7-b076-3e139d640788" />


