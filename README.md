# New Developer Setup

## Things to install before getting started:
- Visual Studio (2022)
- Visual Studio Code
- git
- node.js & npm

## 1 - Setup Github account with company issued email
![Alt text](/imgs/Screen%20Shot%202022-10-03%20at%2013.20.56.png)

## 2 - Generate SSH key
- Open the command prompt on your work computer.
- From within the command prompt run the following:
```
ssh-keygen // creates new SSH key
```
- When you're prompted to "Enter a file in which to save the key", press Enter. This accepts the default file location.
```
Enter file in which to save the key (/home/ash/.ssh/id_rsa):
```
- Next, you will be prompted to enter a secure password. *THIS IS OPTIONAL*
```
Enter passphrase (emtpy for no passphrase):
Enter same passphrase again:
``` 
- You command prompt should looks something like this once completed.
```
Generating public/private rsa key pair.
Enter file in which to save the key (/home/ash/.ssh/id_rsa):
Enter passphrase (emtpy for no passphrase):
Enter same passphrase again:
Your indentification has been saved in /home/ash/.ssh/id_rsa.
Your public key has been saved in /home/ash/.ssh/id_rsa.pub.
The key fingerprint is:
The key's randomart image is:
+--[ED25519 256]--+
|                 |
|                 |
|          .      |
|       .o+       |
|       *S... o o.|
|      o.+o. + E +|
|     o o++.= + B |
|    + +oB** o   .|
|   oo+o*BB+o     |
+----[SHA256]-----+
```
- Once you see the radomart image you have successfully generated your SSH key.
- Now that your SSH key has been generated run the following command to copy it to your clipboard:
```
clip < C:\Users\mike.taft/.ssh/id_ed25519.pub

// the portion 'C:\Users\mike.taft/.ssh/id_ed25519.pub needs to match your SSH key file path. The one shown above is an example. To find your path, scroll up in command prompt to where your SSH key was generated. Look for the text 'Your indentification has been saved in', that is your path to your SSH key.

```

## 3 - Add SSH key to your Github
- Log in to your Github account and go to your settings.

![Alt text](/imgs/Screen%20Shot%202022-10-03%20at%2013.53.04.png)

- Once in the settings window, on the left hand side, click on SSH and GPG Keys. 

![Alt text](/imgs/Screen%20Shot%202022-10-03%20at%2013.53.56.png)

- Click the green button labled 'New SSH Key'

![Alt text](/imgs/Screen%20Shot%202022-10-03%20at%2013.55.24.png)

- Now copy and paste the SSH key you previously copied from command prompt into the textarea labeled 'Key'. You can title the SSH whatever you would like. Example: 'YourName' Work PC

![Alt text](/imgs/Screen%20Shot%202022-10-03%20at%2013.56.22.png)


## 4 - Clone the Anywhere repository to your local machine
