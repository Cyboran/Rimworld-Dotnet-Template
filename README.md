# Rimworld Dotnet Template
A dotnet template for quickly making Rimworld mods via Command line or your favorite IDE.

## Building a DLL Package
To compile the appropriate files, then run the following command: 
```bash
dotnet build ModSource.csproj /p:Configuration=Release /p:RimVersion=1.4
```
or this if you wanted to use the default version
```bash
dotnet build ModSource.csproj /p:Configuration=Release
```
or this if you wanted to use default settings (Debug, Version 1.6)
```bash
dotnet build ModSource.csproj
```

## Getting Started
[Download Git](https://git-scm.com/)

Open Git Bash to where you want to download the files to. 

Clone this project
```bash
git clone https://github.com/Zeta-of-the-rim/Rimwold-Dotnet-Template.git "RimMod"
```

Enter directory
```bash
cd RimMod
```

Add the template
```bash
dotnet new --install .
```

Update the template
```bash
dotnet new --install . --force
```

## Usage
In your Rimworld mod folder, run the following commands:
```bash
mkdir "Your Mod Name"
cd "Your Mod Name"
dotnet new RimMod
```
This will create a new mod with the name you specified.
After that, you can open the project in your favorite IDE and start coding.
I recommend staring by changing the name and author of the mod in the About.xml file.

## Uninstalling
To uninstall the template, run the following command:
```bash
dotnet new --uninstall RimMod
```