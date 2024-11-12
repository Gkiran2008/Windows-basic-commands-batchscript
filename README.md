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
![image](https://github.com/user-attachments/assets/913e66fe-c961-4a10-aa96-2a99ff6dd3d7)

## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
cd %userprofile%\Desktop\MyLab
type nul > MyFile.txt
```
![image](https://github.com/user-attachments/assets/fe66df34-51db-4575-9238-75f22d7fc976)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/user-attachments/assets/ac163f03-7f4f-4f5d-adc6-bfb3bc7ec961)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/user-attachments/assets/dac6b30d-1d5e-45d1-a841-6db6614672ed)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
move MyLab C:\Users\admin\Documents
```

![image](https://github.com/user-attachments/assets/9ec7da92-cde9-4a7d-b970-ca6be001b125)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\DocBackup\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT


![image](https://github.com/user-attachments/assets/398e8e65-5910-43bf-8335-496cb20bcb77)


# RESULT:
The commands/batch files are executed successfully.

