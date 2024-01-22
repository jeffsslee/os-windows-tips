# Useful info for Windows 

## Window Terminal  

### Kinds and Characters

```
CMD
  Meaning : command
  From : Win95-98
  Similar to MS-DOS

Powershell
  From : WinXp

Window Terminal
  BASH job available
```

### How to install (Window Terminal)

> Microsoft Store : Search "Windows Terminal"

## How to set Git Bash into Window Terminal  
> Run Windows Terminal
> To go Settings (or Press Ctrl + ,)
> Press 'Open JSON File
> Add Git Bash Profile into 'profiles'
```
  "profiles": {
    "defaults": {},
    "list": [
      {
        "commandline": "%SystemRoot%\\System32\\WindowsPowerShell\\v1.0\\powershell.exe",
        "guid": "{61c54bbd-c2c6-5271-96e7-009a87ff44bf}",
        "hidden": false,
        "name": "Windows PowerShell"
      },
      {
        "commandline": "%SystemRoot%\\System32\\cmd.exe",
        "guid": "{0caa0dad-35be-5f56-a8ff-afceeeaa6101}",
        "hidden": false,
        "name": "Command Prompt"
      },
      {
        "guid": "{b453ae62-4e3d-5e58-b989-0a998ec441b8}",
        "hidden": false,
        "name": "Azure Cloud Shell",
        "source": "Windows.Terminal.Azure"
      },
      {
        "guid": "{3efe1a20-7b62-4683-89f5-623f1a0feb2e}",
        "hidden": false,
        "name": "Git Bash",
        "commandline": "\"%PROGRAMFILES%\\git\\usr\\bin\\bash.exe\" -i -l",
        "icon": "%PROGRAMFILES%\\git\\mingw64\\share\\git\\git-for-windows.ico",
        "startingDirectory": "%USERPROFILE%",
        "cursorShape": "filledBox"
      }
    ]
  },
```

guid can be generated in the other windows terminal with following code  
```
[guid]::NewGuid()
```

> Save to prifiles and run your window terminal again : you may find Git Bash Link



