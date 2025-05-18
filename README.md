# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.
```
mkdir %userprofile%\Desktop\MyLab
```



## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
![Screenshot 2025-05-18 221417](https://github.com/user-attachments/assets/46fda199-68fb-47ad-9f34-27457e499a90)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-18 221435](https://github.com/user-attachments/assets/b82f63bf-b62b-400c-858f-810f702a93b5)

![Screenshot 2025-05-18 221452](https://github.com/user-attachments/assets/f3e80832-da14-47e8-a2e5-caa302a9c2d1)



## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-18 221509](https://github.com/user-attachments/assets/599b5dec-f76f-4c23-8d2b-51084e4326b4)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![Screenshot 2025-05-18 222336](https://github.com/user-attachments/assets/9f07b010-183a-444d-8d8b-3b844c0063b8)


![Screenshot 2025-05-18 222350](https://github.com/user-attachments/assets/274be4d5-7234-4a1e-9d70-593c272aaca6)


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```

![Screenshot 2025-05-18 222403](https://github.com/user-attachments/assets/71544048-e754-41b8-a064-d8c337a06de4)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```

## OUTPUT

![Screenshot 2025-05-18 222413](https://github.com/user-attachments/assets/69a1edaa-93d0-484e-8c62-7e2596915bea)





# RESULT:
The commands/batch files are executed successfully.

