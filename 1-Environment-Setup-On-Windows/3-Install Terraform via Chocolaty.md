# Install Visual Studio Code, Terraform and Set the PATH Using Chocolatey

Chocolatey is a popular package manager for Windows which can simplify the installation of software like Visual Studio Code and Terraform.

**Note:** You need to have administrative privileges on your computer to install Chocolatey and use it to install packages.

## Install Chocolatey

1. Open PowerShell as an Administrator (right-click the PowerShell application and select 'Run as Administrator').
2. Run the following command:

    ```powershell
    Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
    ```
3. Close the PowerShell.

## Install Visual Studio Code

1. Open a new PowerShell as an Administrator.
2. Run the following command:

    ```powershell
    choco install vscode
    ```
This will install Visual Studio Code using Chocolatey.

## Install Terraform

1. In the same PowerShell window, run the following command:

    ```powershell
    choco install terraform
    ```
This will install Terraform using Chocolatey. The installation should automatically add Terraform to your system's PATH, so you don't need to do it manually.

## Verify the Installations

You can verify the installations by running the following commands:

- For Visual Studio Code:

    ```powershell
    code
    ```
This should open Visual Studio Code.

- For Terraform:

    ```powershell
    terraform
    ```
You should see a list of available Terraform commands, which confirms that Terraform has been successfully installed.
