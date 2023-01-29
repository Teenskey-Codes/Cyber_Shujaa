___

## **WINDOWS MANAGEMENT INSTRUMENTATION**
___

- Get-WmiObject 
    -  is a command in PowerShell, which is a command-line interface for Windows operating system. The command is used to retrieve information about the WMI (Windows Management Instrumentation) objects on a local or remote computer. WMI is a technology that allows you to manage and monitor various aspects of your computer such as hardware, software, and security-related information.

    - The "Get-WmiObject" command is used to access information stored in WMI, it allows you to query the WMI repository and retrieve specific information about the different hardware and software components of your computer, such as the manufacturer, model, version of the operating system, installed programs, battery status, and more.

    - In summary, "Get-WmiObject" is a command that helps you access the WMI objects on your computer, it is a powerful tool that can help you retrieve information about your computer and its components, troubleshoot problems, and monitor your computer's performance and security.


___

## **WINDOWS MANAGEMENT INSTRUMENTATION COMMANDS**
___

1. "Get-WmiObject -Class Win32_ComputerSystem" - This command will give you information about your computer's hardware like the manufacturer, model, and number of processors.

2. "Get-WmiObject -Class Win32_OperatingSystem" - This command will give you information about the operating system installed on your computer like the version, build number, and the last time it was started.

3. "Get-WmiObject -Class Win32_Product" - This command will give you a list of all the software programs installed on your computer.

4. "Get-WmiObject -Class Win32_Battery" - This command will give you information about the battery of your computer, like the power state, capacity, and the number of charge cycles.

5. "Get-WmiObject -Class Win32_NetworkAdapter" - This command will give you information about your computer's network adapters, like the name, MAC address, and the status of the adapter.

- These are just a few examples, but there are many other classes of information that you can access with "Get-WmiObject" command. This command is useful for getting information about the different hardware and software components on your computer, and can be helpful when troubleshooting problems or gathering information for audits.






