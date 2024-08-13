# Install & Configure Helm

## Step-01: Install Helm

- Navigate to Helm official documentation: https://helm.sh/docs/intro/install/

### 1.1 On Windows (using chocolatey package manager)

- First, install **Chocolatey package manager** as a prerequisite.
- Ref: https://chocolatey.org/install#individual

- On your local system, launch **Powershell** as an _administrator_.
- Next, ensure that the result of **Get-ExecutionPolicy** is not _Restricted_.
- You may Bypass the policy to get things installed or _AllSigned_ for quite a bit more security.

```
Get-ExecutionPolicy

[If it returns RemoteSigned, you're good to move to next step]
[If it returns Restricted, then run following command]

Set-ExecutionPolicy AllSigned

OR

Set-ExecutionPolicy Bypass -Scope Process
```

- Install chocolatey package manager

```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))

[Wait a few seconds for the command to complete]
```

- To confirm the successful installation, check the installed version of chocolatey:

```
choco --version
```

- Now, use** chocolatey package manager to install Helm**

```
choco install kubernetes-helm

# To confirm the successful helm installation, check the version
helm version
```
