# Pre-Compiled Binaries <a name="top"></a>
To go back to the Unit 4 Project, click [here](/Unit-4/README.md).  
To go back to the main APCSP repo, click [here](/README.md).

---

## 64-bit vs 32-bit
Before you select a download, please make sure you know whether you have a 32-bit machine or a 64-bit machine. This will allow you to select the correct download. If you do not know what type of machine you have or you do not know how to check, the 32-bit downloads will work on both types of machines.

**Note:** Downloads are not avaliable for other types of machines, such as ARM, or for Apple machines. If you do not have a 32-bit machine or a 64-bit machine which runs Windows or Linux, you will need to compile the binaries yourself from the source code.

---

## Windows Users
### Installers
Click [here](./Unit-4-win-x86-64-installer.exe) to download the 64-bit installer.  
Click [here](./Unit-4-win-x86-installer.exe) to download the 32-bit installer.  
Click [here](#win-installer) for installation instructions.

### .NET-Dependent Binaries ([What is this?](#dotnet-dependency))
Click [here](./Unit-4-win-x86-64-dotnet.exe) to download the 64-bit pre-compiled .NET-dependent binary.  
Click [here](./Unit-4-win-x86-dotnet.exe) to download the 32-bit pre-compiled .NET-Dependent binary.  
Click [here](#win-install-dotnet) for installation instructions.

### Standalone Binaries ([What is this?](#dotnet-dependency))
Click [here](./Unit-4-win-x86-64-standalone.exe) to download the 64-bit pre-compiled standalone binary.  
Click [here](./Unit-4-win-x86-standalone.exe) to download the 32-bit pre-compiled standalone binary.  
Click [here](#win-install-standalone) for installation instructions.

---

## Linux Users
### .NET-Dependent Binaries ([What is this?](#dotnet-dependency))
Click [here](./Unit-4-linux-x86-64-dotnet) to download the 64-bit pre-compiled .NET-dependent binary.  
Click [here](./Unit-4-linux-x86-dotnet) to download the 32-bit pre-compiled .NET-dependent binary.  
Click [here](#linux-install-dotnet) for installation instructions.

### Standalone Binaries ([What is this?](#dotnet-dependency))
Click [here](./Unit-4-linux-x86-64-standalone) to download the 64-bit pre-compiled standalone binary.  
Click [here](./Unit-4-linux-x86-standalone) to download the 32-bit pre-compiled standalone binary.  
Click [here](#linux-install-standalone) for installation instructinons.

---

# Installation Instructions
## Windows Installer <a name="win-installer"></a>
1. Download the appropriate installer for your machine (32-bit or 64-bit).
    - Your browser may tell you that applications downloaded from the internet can harm your computer. Ignore this warning and proceed with the download.
2. Double-click the downloaded application to run it. It will open an install wizard.
    - Your machine may inform you that the application could be harmful. Ignore this warning. Press `More Info`, and then press `Run Anyway`. [Why does this happen?](/README.md#why-the-warning)
3. Follow the instructions in the install wizard. It will guide you through installing the application, and then run the application once you're done.
4. You're all set!
    - To run the application again, double-click the shorcut on your desktop.
    - Use the command `help` to view a list of the avaliable commands.

#### Important Note:
The installer does not come with an uninstaller. In the event that you wish to remove the application from your device, you will need to use the File Explorer application to manually delete the folder application folder and its contents. The folder will either be located at `C:\Program Files\Unit 4\` or `C:\Program Files (x86)\Unit 4\`.

## Windows .NET-Dependent Binaries <a name="win-install-dotnet"></a>
1. Download and install the .NET Runtime. (Skip this step if you already have it installed)  
For 64-bit machines, use [this link](https://dotnet.microsoft.com/download/dotnet/thank-you/runtime-desktop-5.0.0-windows-x64-installer).  
For 32-bit machines, use [this link](https://dotnet.microsoft.com/download/dotnet/thank-you/runtime-desktop-5.0.0-windows-x86-installer).
2. Download the appropriate .NET-dependent binary (32-bit or 64-bit).
    - Your browser may tell you that applications downloaded from the internet can harm your computer. Ignore this warning and proceed with the download.
3. Create a new folder on your desktop. Name it something that will help you remember what it's for, such as `Unit 4`.
4. Cut and paste the binary you downloaded in step 2 into the folder you created in step 3.
5. (Optional) Right-click the application and then click `Create Shortcut`. Cut and paste the new shortcut to your Desktop folder.
6. Double-click the application to run it.
    - This step will create a file called `gamedata` within the folder. This file contains information such as player's highscores. Never delete the `gamedata` file while the application is running, and never modify the contents of the file. If you do delete the `gamedata` file by accident, just run the application again - it will generate a new one.
    - The first time you run the application, your machine may inform you that the application could be harmful. This will only happen once. Press `More Info`, and then press `Run Anyway`. [Why does this happen?](/README.md#why-the-warning)
7. You're all set!
    - Double-click the application or the shortcut to run it again.
    - Enter the command `help` to view a list of avaliable commands.

## Windows Standalone Binaries <a name="win-install-standalone"></a>
1. Download the appropriate standalone binary (32-bit or 64-bit).
    - Your browser may tell you that applications downloaded from the internet can harm your computer. Ignore this warning and proceed with the download.
2. Create a new folder on your dekstop. Name it something that will help you remember what it's for, such as `Unit 4`.
3. 
3. Cut and paste the application you downloaded in step 1 into the folder you created in step 2.
4. (Optional) Right-click the application and then click `Create Shortcut`. Cut and paste the new shortcut to your Desktop folder.
5. Double-click the application to run it.
    - This step will create a file called `gamedata` within the folder. This file contains information such as player's highscores. Never delete the `gamedata` file while the application is running, and never modify the contents of the file. If you do delete the `gamedata` file by accident, just run the application again - it will generate a new one.
    - The first time you run the application, your machine may inform you that the application could be harmful. This will only happen once. Press `More Info`, and then press `Run Anyway`. [Why does this happen?](/README.md#why-the-warning)
6. You're all set!
    - Double-click the application or the shortcut to run it again.
    - Enter the command `help` to view a list of avaliable commands.

## Linux .NET-Dependent Binaries <a name="linux-install-dotnet"></a>
1. Download and install the .NET runtime. (Skip this step if you already have it installed)  
Follow the instructions at [this](https://docs.microsoft.com/en-us/dotnet/core/install/linux) website.
2. Download the appropriate .NET-dependent binary (32-bit or 64-bit). Make sure it saves to your Downloads folder.
    - Your browser may tell you that applications downloaded from the internet can harm your computer. Ignore this warning and proceed with the download.
3. Open a new terminal prompt and run the appropriate command based on which binary you downloaded.  
64-bit Binaries:  
`mkdir ~/Unit-4/ && cp ~/Downloads/Unit-4-linux-x86-64-dotnet ~/Unit-4/ && chmod +x ~/Unit-4/Unit-4-linux-x86-64-dotnet && echo "alias unit4='~/Unit-4/Unit-4-linux-x86-64-dotnet'" >> ~/.bashrc`  
32-bit Binaries:  
`mkdir ~/Unit-4/ && cp ~/Downloads/Unit-4-linux-x86-dotnet ~/Unit-4/ && chmod +x ~/Unit-4/Unit-4-linux-x86-dotnet && echo "alias unit4='~/Unit-4/Unit-4-linux-x86-dotnet'" >> ~/.bashrc`
4. Close the terminal prompt, and then open a new one.
5. You're all set!
    - To run the application, run the command `unit4` from any terminal prompt.
    - Once you run the application, run the command `help` to view a list of avaliable commands.


## Linux Standalone Binaries <a name="linux-install-standalone"></a>
1. Download the appropriate standalone binary (32-bit or 64-bit). Make sure that it saves to your Downloads folder.
    - Your browser may tell you that applications downloaded from the internet can harm your computer. Ignore this warning and proceed with the download.
2. Open a new terminal prompt and run the appropriate command based on which binary you downloaded.  
64-bit Binaries:  
`mkdir ~/Unit-4/ && cp ~/Downloads/Unit-4-linux-x86-64-standalone ~/Unit-4/ && chmod +x ~/Unit-4/Unit-4-linux-x86-64-standalone && echo "alias unit4='~/Unit-4/Unit-4-linux-x86-64-standalone'" >> ~/.bashrc`  
32-bit Binaries:  
`mkdir ~/Unit-4/ && cp ~/Downloads/Unit-4-linux-x86-standalone ~Unit-4/ && chmod +x ~/Unit-4/Unit-4-linux-x86-standalone && echo "alias unit4='~/Unit-4/Unit-linux-x86-standalone'" >> ~/.bashrc`
3. Close the terminal prompt, and then open a new one.
4. You're all set!
    - To run the application, run the command `unit4` from any terminal prompt.
    - Once you run the application, run the command `help` to view a list of avaliable commands.

---

[Back to Top](#top)
