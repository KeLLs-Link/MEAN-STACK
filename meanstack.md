# **Objective**
- **Implementing a simple Book Register web form using MEAN STACK on Ubuntu Server deployed on AWS**

```
sudo apt update
```
```
sudo apt upgrade
```

- **Add certificates**

SSL/TLS certificates play a critical role in ensuring the security, authentication, privacy, and trustworthiness of websites on the internet, making them essential for safeguarding sensitive online transactions and communications.

```
sudo apt -y install curl dirmngr apt-transport-https lsb-release ca-certificates
```
***curl:*** A command-line tool for transferring data using various network protocols.

***dirmngr:*** A server for managing and downloading OpenPGP keys from key servers.

***apt-transport-https:*** A package that allows apt to fetch packages over HTTPS.

***lsb-release:*** A package providing information about the Linux Standard Base (LSB) release.

***ca-certificates:*** A package containing public CA certificates used for verifying the authenticity of SSL connections.
```
curl -sL https://deb.nodesource.com/setup_18.x | sudo -E bash -:
```
This command uses curl to download a script from https://deb.nodesource.com/setup_18.x.

***The -s flag*** tells curl to work silently without showing progress or errors.

***The -L*** flag tells curl to follow HTTP redirects if the server responds with a redirect.

The downloaded script is then piped (|) to bash, a shell interpreter, to be executed.

***The -E flag*** for sudo preserves the user's environment when running the subsequent command (bash -).

This script adds the NodeSource repository for Node.js to the system's package sources, making it possible to install Node.js version 12.x using apt after this setup.

***In summary, these commands install some prerequisite packages required for package management and then set up the Node.js repository for installing Node.js version 12.x on the Ubuntu system.***

![image](./Images/repositoryconfig.png)

- **Install NodeJs**

Node.js is a JavaScript runtime built on Chrome’s V8 JavaScript engine. Node.js is used in this tutorial to set up the Express routes and AngularJS controllers.
Update Ubuntu.
```
sudo apt install -y nodejs
```
![image](./Images/nodejs.png)

