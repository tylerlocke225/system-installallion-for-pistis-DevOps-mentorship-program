# system-installallion-for-pistis-DevOps-mentorship-program
OpenSSH is a suite of secure networking utilities based on the SSH protocol.This repository provides documentation for installing, configuring, and using OpenSSH on Windows.
system installation for pistis DevOps mentorship program.

overview.

1.install choco package manager

2.install git bash

3.install vs code

4.install OpenSSH sever
1. install choco package manager. a. by using powershell

Open PowerShell as Administrator: Search for PowerShell, right-click on it, and select "Run as Administrator".

Set Execution Policy: You may need to set the execution policy to allow running scripts. Enter the following command: command: Set-ExecutionPolicy Bypass -Scope Process -Force

Install Chocolatey: Run the installation command for Chocolatey:

command: iex "& { $(irm https://chocolatey.org/install.ps1 -UseBasicP) }"

Verify Installation: Once the installation is complete, you can verify it by checking the Chocolatey version:

command: choco --version That's it! Chocolatey should now be installed on your system.

2. install git bash search for 'install git bash' then you will see a website like the image below image then you click on it and it is going to bring this image then you pick the type of laptop\desktop you are using

3. install vs code search for 'install vs code' then you will see a website like the image below image then you click on it and it is going to bring this image then you pick the type of laptop\desktop you are using.

4. install of OpenSSH sever using powershell

Open PowerShell as Administrator: Search for Powershell, right-click on it, and select "Run as Administrator".

Install OpenSSH Server: Use the Add-WindowsCapability cmdlet to install the OpenSSH Server feature. Run the following command: command: Add-WindowsCapability -Online -Name OpenSSH.Server~~~~0.0.1.0

Start and Configure the SSH Server:

Start the SSH server

command: Start-Service sshd Set the SSH server to start automatically with Windows command: Set-Service -Name sshd -StartupType 'Automatic' Confirm Installation: To verify that the OpenSSH Server is installed and running, you can use: command: Get-Service -Name sshd
