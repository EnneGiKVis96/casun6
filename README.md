
# Casun6

Winget | Windows Updates | Since 2023.
Casun6 is a Powershell Script to simplify the package manager winget and create a single unified CLI for packages and system updates.

## Installation

Install casun6 script with Powershell

```bash
  Install-Script -Name casun6
```
It will install the script and his dependency: Microsoft.WinGet.Client

## Update

You can update casun6 in the same way using Powershell

```bash
  Update-Script -Name casun6
```


## Features 

- Install winget packages 
- Update winget packages 
- List intalled winget packages
- Find packages in the winget repos
- Exclude and include packages from updating
- Update Windows with system updates


## Usage/Examples

Check all available commands:
```powershell
casun6 -H 
```

Install a package from winget:
```powershell
casun6 -I WinSCP.WinSCP
casun6 -I WinSCP.WinSCP -V 6.1.1 # You can specify the version if available
```

Update packages and/or Windows:
```powershell
casun6 -U # Update only winget packages
casun6 -W # Update only Windows REQUIRE ADMIN PERMISSION
casun6 -W -O # Include optional Windows updates -> REQUIRE ADMIN PERMISSION
casun6 -A # Update for winget packages and Windows updates -> REQUIRE ADMIN PERMISSION
casun6 -A -N # It also includes optional updates -> REQUIRE ADMIN PERMISSION

```

Find any package in the winget repos
```powershell
casun6 -F WinSCP 
```

Remove a package from your system:
```powershell
casun6 -R WinSCP.WinSCP 
```

List your installed packages
```powershell
casun6 -L
```

Exclude a package / include a package previously excluded
```powershell
casun6 -E WinSCP.WinSCP # To exclude
casun6 -P WinSCP.WinSCP # To include back
```


## Screenshots

![App Screenshot](https://snipboard.io/8SzWoZ.jpg)

![App Screenshot](https://snipboard.io/eFyLWJ.jpg)

![App Screenshot](https://snipboard.io/K49Htx.jpg)

