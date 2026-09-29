# Apache for Amazon-Linux
Apache in Amazon linux is refferd as httpd. This is the installation guide for installing httpd in amazon Linux.

## Step for installing httpd.
### Step 1: First you have to check the package is available or not.
```
  httpd --version
```

<img width="635" height="118" alt="image" src="https://github.com/user-attachments/assets/bf410429-bb05-4e31-9db3-576a92eeb43f" />

### Step 2: Now enter the command for installing
```
  sudo dnf install httpd
```

<img width="635" height="118" alt="image" src="https://github.com/user-attachments/assets/d44ce55a-b36a-4972-88a0-9e3310b3ca7d" />

### Step 3: Verify
```
  which httpd
```

<img width="1001" height="90" alt="image" src="https://github.com/user-attachments/assets/2b5ef2a2-1aad-4f07-abde-cfd621d81369" />


### Step 4: Check status
```
  sudo systemctl status httpd
```

<img width="1303" height="147" alt="image" src="https://github.com/user-attachments/assets/6a44d337-d379-4055-b451-c3c267597481" />

### Step 5: Start the service and then check the status
```
  sudo systemctl start httpd
```
```
  sudo systemctl status httpd
```

<img width="1006" height="391" alt="image" src="https://github.com/user-attachments/assets/bb4422b0-f487-41e5-99b0-eba519b2bacd" />

### Step 6: Enable the service and then check the status
This will start the service automatically when the machine or server will restart.
```
  sudo systemctl enable httpd
```
```
  sudo systemctl status httpd
```

<img width="1000" height="396" alt="image" src="https://github.com/user-attachments/assets/c03df06d-147d-4d10-a538-7c041b4f6a71" />

