___
# POWERSHELL ALIASES
___

1. pwd = Get-Location - displays the current location (directory) you are in.

Example: pwd

2. ls = Get-ChildItem - lists the files and folders in the current directory.

Example: ls

3. cd = Set-Location - changes the current directory you are in.

Example: cd c:\users\username\documents

4. dir = Get-ChildItem - lists the files and folders in the current directory.

Example: dir

5. mkdir = New-Item -ItemType Directory - creates a new directory (folder)

Example: mkdir newfolder

6. rmdir = Remove-Item -Force -Recurse - deletes a directory (folder) and all its contents.

Example: rmdir oldfolder -force -recurse

7. rm = Remove-Item -Force - deletes a file or directory.

Example: rm file.txt -force

8. cp = Copy-Item - copies a file or directory to a new location.

Example: cp file.txt c:\backup

9. mv = Move-Item - moves a file or directory to a new location.

Example: mv file.txt c:\backup

10. gci = Get-ChildItem - lists the files and folders in the current directory.

Example: gci

11. pushd = Push-Location - saves the current location (directory) you are in and changes to a new one.

Example: pushd c:\users\username\documents

12. popd = Pop-Location - goes back to the last saved location (directory) you were in.

Example: popd

13. touch = New-Item -ItemType File - creates a new file.

Example: touch newfile.txt

14. del = Remove-Item -Force - deletes a file or directory.

Example: del file.txt -force

15. copy = Copy-Item - copies a file or directory to a new location.

Example: copy file.txt c:\backup

16. move = Move-Item - moves a file or directory to a new location.

Example: move file.txt c:\backup

17. md = New-Item -ItemType Directory - creates a new directory (folder)

Example: md newfolder

18. rd = Remove-Item -Force -Recurse - deletes a directory (folder) and all its contents.

Example: rd oldfolder -force -recurse

19. echo = Write-Output - writes a message or value to the screen.

Example: echo "Hello World"

20. cat = Get-Content - displays the contents of a file.

Example: cat file.txt

21. more = Select-Object -First X -ExpandProperty - Displays the contents of a file one page at a time.

Example: get-content file.txt | more

22. clear = Clear-Host - Clear the console screen.

23. cls = Clear-Host - Clear the console screen.

Example: cls

24. exit = Exit-PSSession - Close the PowerShell session

Example: exit

25. chdir = Set-Location - changes the current directory you are in.

Example: chdir c:\users\username\documents

26. type = Get-Content - displays the contents of a file.

Example: type file.txt

27. find = Select-String - find and display specified text in files.
Example: get-content file.txt | select-string -pattern "text to find"

28. findstr = Select-String - find and display specified text in files.

29. Example: get-content file.txt | select-string -pattern "text to find"

30. where = Where-Object - filter the output of a command based on specified conditions.

Example: get-process | where name -eq "powershell"

31. sort = Sort-Object - sorts the output of a command based on specified conditions.

Example: get-process | sort -property name

32. measure = Measure-Object - provides statistics about the output of a command, such as count, sum, minimum, and maximum.

Example: get-process | measure-object

33. group = Group-Object - groups the output of a command based on specified properties.

Example: get-process | group-object -property name

34. select = Select-Object - select specific properties of the output of a command.

Example: get-process | select-object -property name,id

35. out-file = Out-File - sends the output of a command to a file.

Example: get-process | out-file processes.txt

36. out-gridview = Out-GridView - displays the output of a command in a grid view.

Example: get-process | out-gridview

37. format-table = Format-Table - formats the output of a command as a table.

Example: get-process | format-table -property name,id

38. gwmi = Get-WmiObject - Retrieves WMI class information from a specified computer.

Example: gwmi -class win32_operatingsystem -computer "localhost"

39. invoke-command = Invoke-Command - Runs commands on local and remote computers.

Example: invoke-command -computer "remote-computer" -scriptblock {get-process}

40. start-transcript = Start-Transcript - starts a transcript of a PowerShell session.
Example: Start-Transcript -path "c:\logs\session.log"

41. stop-transcript = Stop-Transcript - stops a transcript of a PowerShell session.
Example: Stop-Transcript