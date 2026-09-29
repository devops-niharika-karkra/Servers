# Apache Installation In Ubuntu
In ubuntu, Apache is reffered as Apache2. This is the installation guide for installing apache2 using linux commands.

## Steps for installation:-
### Step 1: Check if apache is already installed.
### Command: 
```
  apache2 --version
```

<img width="771" height="136" alt="image" src="https://github.com/user-attachments/assets/2e8ba9d9-c1b1-4223-b058-df773a1c9af6" />

### Step 2: Update packages of apt to fetch the latest version using command:
```
  sudo apt update
```

<img width="1002" height="300" alt="image" src="https://github.com/user-attachments/assets/49019b06-4977-462e-b670-4147411ed0c1" />

### Step 3: To install, enter command 
### Command:
```
  sudo apt install apache2
```

<img width="1001" height="443" alt="image" src="https://github.com/user-attachments/assets/2f50dafb-eba3-4223-890a-020c0bdd4c3a" />

### Step 4: Verify, whether the apache is installed and running.
### Command:
```
  sudo systemctl status apache2
```

<img width="1002" height="300" alt="image" src="https://github.com/user-attachments/assets/a6fd5c62-39b8-4cfa-86da-83116f8b3138" />

