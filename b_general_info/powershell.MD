___ 

## **POWER SHELL COMMANDS**
___


#### USEFUL COMMANDS TO KNOW
- **get-alias** -
    is used to display a list of all the available aliases in the current session. An alias in PowerShell is a shortcut for a cmdlet or command. Aliases are used to create a more convenient or familiar way to run a command.

- **get-help alias-name** 
    Get-Help ls (assuming that ls is an alias for Get-ChildItem), it will display information about the Get-ChildItem cmdlet, including its syntax, parameters, and examples of how to use it. This can be useful if you're not familiar with the cmdlet or command that an alias represents, or if you want to learn more about a specific aspect of the cmdlet or command.

    ##### Example

    ```powershell
    get-help sl
    ```
        NAME
            Set-Location

        SYNOPSIS
            Sets the current working location to a specified location.


        SYNTAX
        Set-Location -LiteralPath <System.String> [-PassThru] [-UseTransaction]
        [<CommonParameters>]

        Set-Location [[-Path] <System.String>] [-PassThru] [-UseTransaction] [<CommonParameters>]

        Set-Location [-PassThru] [-StackName <System.String>] [-UseTransaction]
        [<CommonParameters>]


        DESCRIPTION
            The `Set-Location` cmdlet sets the working location to a specified location. That
            location could be a directory, a subdirectory, a registry location, or any provider path.

            You can also use the StackName parameter to make a named location stack the current
            location stack. For more information about location stacks, see the Notes. 


    


- **Get-Alias -Name "alias_name** -
    to see information about a specific alias. For example, you can use Get-Alias -Name ls to see information about the ls alias.

___
### Common Powershell Commands

___

1. Get-Process: This command retrieves a list of all running processes on the computer. The verb "Get" retrieves information, and the noun "Process" specifies that the command should retrieve information about running processes.

2. Stop-Process -Name "chrome": This command stops the process with the name chrome. The verb "Stop" stops a process and the noun "Process" specifies that the command should be used to stop a process. The -Name flag with the "chrome" value specify the process to be stopped.
```powershell
# To stop Visual Studio Code From Running
Stop-Process -Name "Code"

# The -Name flag specifies the process name and the value "Code" or "Code.exe" is the process name of VSCode.

# It's important to note that this will close any instance of VSCode that you have open, and any unsaved changes will be lost. Additionally, this command will not prompt the user for confirmation before stopping the process, so if you're not sure if you want to stop the process, you can use Get-Process command to see what processes are running and check if it's running before using Stop-Process command.


```


3. Get-Service: This command retrieves a list of all installed services on the computer. The verb "Get" retrieves information, and the noun "Service" specifies that the command should retrieve information about installed services.

- Installed Services 
        -These are the background processes or daemons that run on a Windows computer. These services provide the underlying functionality for many of the features and functions of the operating system, such as the ability to connect to a network, manage users and permissions, and perform tasks on a schedule.

        Services are typically installed with the operating system, or with software that you install on your computer. They are different from applications, which are programs that you interact with directly, services are running in the background and can be started, stopped, paused and restarted, they provide features and capabilities to different parts of the operating system and the applications that runs on it.

        The Get-Service command in PowerShell retrieves a list of all services that are currently installed on the computer and their current status, it will display the Name, DisplayName, Status, StartupType, and other information of the services installed on your computer.

        Some examples of installed services are the DNS client service, the DHCP client service, the Windows Update service, and many others. These services are not visible on the computer but they run in the background and perform important tasks to keep the operating system running smoothly.
```powershell

# # PS C:\Windows\system32> 
Get-Service                                                           
# Status   Name               DisplayName
# ------   ----               -----------
# Stopped  AarSvc_2b32d8      Agent Activation Runtime_2b32d8
# Stopped  AJRouter           AllJoyn Router Service

```
4. Start-Service -Name "DNS": This command starts the service with the name DNS. The verb "Start" starts a service and the noun "Service" specifies that the command should be used to start a service. The -Name flag with the "DNS" value specifies the service to be started.

####   Examples of Common Services that can be started in powershell

    1. "DNS Client": This service resolves DNS names to IP addresses. When you type a web address into your browser, your computer sends a request to the DNS client service to find the IP address of the website you want to visit.

    2. "Windows Update": This service checks for and installs updates to the operating system. This service can be used to check and install important updates like security fixes, feature updates, etc.

    3. "Remote Desktop Services": This service allows users to connect to the computer remotely using Remote Desktop Protocol (RDP) which provides a graphical interface to connect to another computer over a network connection.

    4. "Print Spooler": This service manages print jobs that are sent to a printer. It helps to ensure that print jobs are sent to the printer in the correct order and that the printer does not become overwhelmed with too many jobs at once.

    5. "Themes": This service manage the visual presentation of the Operating System, it manages desktop background, window color, and sounds.

    6. "Windows Management Instrumentation": This service provides management information and control for systems using the Windows Management Instrumentation infrastructure.

    7. "Remote Registry": This service allows remote access to the registry, it can be helpful for administrator to manage the registry of a remote computer, but it also can introduce a security vulnerability if not properly configured.

5. Get-ChildItem -Path "C:\Windows\System32": This command retrieves a list of all files and folders in the "C:\Windows\System32" directory. The verb "Get" retrieves information, and the noun "ChildItem" specifies that the command should retrieve information about files and folders. The -Path flag with the value "C:\Windows\System32" specifies the directory that the command should retrieve information from.

6. Remove-Item -Path "C:\temp\tempfile.txt": This command deletes the file "tempfile.txt" in the "C:\temp" directory. The verb "Remove" deletes an item, and the noun "Item" specifies that the command should be used to delete a file. The -Path flag with the value "C:\temp\tempfile.txt" specifies the file that the command should delete.

7. Get-Location: This command displays the current working directory, also known as the current directory, or the current location, in the file system.

8. Set-Location: This command changes the current working directory. For example, Set-Location C:\Windows would change the current directory to the Windows folder on the C drive.

9. Get-ChildItem: This command lists the files and directories in the current working directory. You can also specify a path to list the files and directories in a different directory. For example, Get-ChildItem C:\Windows would list the files and directories in the Windows folder on the C drive.

10. Move-Item : This command allows you to move files and folders to a different location. The syntax is: Move-Item -Path "path of the item" -Destination "path of the destination" for instance Move-Item -Path "C:\example\file.txt" -Destination "C:\example2" would move the file.txt from the folder example to the folder example2

11. Copy-Item : This command allows you to copy files and folders to a different location. The syntax is: Copy-Item -Path "path of the item" -Destination "path of the destination" for instance Copy-Item -Path "C:\example\file.txt" -Destination "C:\example2" would copy the file.txt from the folder example to the folder example2

12. Remove-Item : This command allows you to delete files and folders. The syntax is: Remove-Item -Path "path of the item" for instance Remove-Item -Path "C:\example\file.txt" would delete the file.txt from the folder example

13. New-Item : This command allows you to create new files or folders. The syntax is: New-Item -Path "path of the item" -ItemType file/directory for instance New-Item -Path "C:\example\newfolder" -ItemType directory would create a new folder called newfolder in the example folder