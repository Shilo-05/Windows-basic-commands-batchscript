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


## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/YASHWINISEC/Windows-basic-commands-batchscript/assets/139361633/ebb98d97-daa3-4017-b79f-5aa0d7788602)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT

cd %userprofile%\Desktop\MyLab

![image](https://github.com/YASHWINISEC/Windows-basic-commands-batchscript/assets/139361633/6b299cb4-ab1f-4430-a0a7-cb9fdda3dd72)

![image](https://github.com/YASHWINISEC/Windows-basic-commands-batchscript/assets/139361633/9763be10-6649-4fbd-9ffd-32c1e8e56a74)

List the contents of the "MyLab" directory.

## COMMAND AND OUTPUT

dir %userprofile%\Desktop\MyLab

![image](https://github.com/YASHWINISEC/Windows-basic-commands-batchscript/assets/139361633/a90d1460-cabf-45b1-897d-7a67ca167442)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/YASHWINISEC/Windows-basic-commands-batchscript/assets/139361633/bb543224-3070-43b7-9b86-9503ac5d7986)

![image](https://github.com/YASHWINISEC/Windows-basic-commands-batchscript/assets/139361633/3c22d688-8b79-4dde-a15f-0bfc8083e1c3)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents
![image](https://github.com/YASHWINISEC/Windows-basic-commands-batchscript/assets/139361633/3553b937-a549-450f-8e13-11cbce2de4ee)

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
![image](https://github.com/YASHWINISEC/Windows-basic-commands-batchscript/assets/139361633/eae8a2b4-e5bf-4e0e-b4dd-cda8d8678984)

# RESULT:
The commands/batch files are executed successfully.

