# powershell-layout


## About

This folder has been created to setting a powershell terminal
with colors like this:

![MyPowershell][img-mypowershell]


## Prerequisites

- Install [posh-git](https://github.com/dahlbyk/posh-git) module
- Download and Install [ColorTool](https://github.com/microsoft/terminal/releases/tag/1904.29002)
- Setting a [Profile.ps1](https://ss64.com/ps/syntax-profile.html)
- Install [Dracula Theme from powershell](https://github.com/dracula/powershell/blob/master/INSTALL.md)
- Installl [oh-my-posh](https://github.com/JanDeDobbeleer/oh-my-posh)
- Uses [Meslo LG M Regular for Powerline Nerd Font](https://github.com/ryanoasis/nerd-fonts/releases/download/v2.1.0/Meslo.zip) from [Nerd Fonts](https://www.nerdfonts.com/font-downloads)

## Installation

Install posh-git module:

- run `Set-ExecutionPolicy RemoteSigned -scope CurrentUser`   and after `Install-Module posh-git -Scope CurrentUser`



Download and Install ColorTool 

- Click on [Download ColorTool Link](https://raw.githubusercontent.com/waf/dracula-cmd/master/dist/ColorTool.zip)

- Open PowerShell, navigate to the unzipped ColorTool directory, and run install.cmd.



Setting a Profile.ps1

- Open PowerShell 

- Run `notepad $Profile`

- Put inside Profile.ps1 this configuration [dracula_prompt-configutarions.ps1](https://github.com/dracula/powershell/blob/master/theme/dracula-prompt-configuration.ps1) and save

- Run `.$Profile` on PowerShell to reload the profile into the current session


Install oh-my-posh

- Run `Install-Module -Name oh-my-posh -RequiredVersion 2.0.492	`

- Run `notepad $Profile`  add this configuration and save:

```
#oh-my-posh Setup
if (!(Test-Path -Path $PROFILE )) { New-Item -Type File -Path $PROFILE -Force }

#oh-my-posh Import
Import-Module oh-my-posh

#oh-my-posh Theme 
Set-Theme Zash

```

- Run `.$Profile` on PowerShell to reload the profile into the current session

Uses Meslo LG M Regular for Powerline Nerd Font

- Click here [Download Meslo Link](https://github.com/ryanoasis/nerd-fonts/releases/download/v2.1.0/Meslo.zip)

- Unzip and search `Meslo LG M Regular Nerd Font Complete Windows Compatible.ttf` to install 

- Open PowerShell and with right click at toolball choose Properties and select Fonts just like that:

    ![PowershellConfigs][img-powershellconfigs]


    🎉 Just Enjoy It! 🥰


[img-mypowershell]: img/mypowershell.png
[img-powershellconfigs]: img/powershellconfigs.png
