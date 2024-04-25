# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript
DEVELOPED BY:GOKUL S
REGISTER NO:212223040051

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

![image](https://github.com/SGokul2005/Windows-basic-commands-batchscript/assets/147121825/b0766dce-2000-4519-9503-71debd32dce6)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![image](https://github.com/SGokul2005/Windows-basic-commands-batchscript/assets/147121825/1eb1c657-c2ce-4e25-be86-3e2eb478920c)


![image](https://github.com/SGokul2005/Windows-basic-commands-batchscript/assets/147121825/487d9d05-7470-434e-b24e-19aefdc3ab36)

List the contents of the "MyLab" directory.
## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/SGokul2005/Windows-basic-commands-batchscript/assets/147121825/f9c1282b-d85c-43c3-9353-0873706d5e6c)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/SGokul2005/Windows-basic-commands-batchscript/assets/147121825/6212176a-23ff-456a-80dd-2a62c2927e08)

![image](https://github.com/SGokul2005/Windows-basic-commands-batchscript/assets/147121825/2518094e-0b7e-4c65-8b14-046461f76e08)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents

![image](https://github.com/SGokul2005/Windows-basic-commands-batchscript/assets/147121825/72560b1f-0874-4c3f-96ec-e6474f5e1ab2)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
~~~
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
~~~
## OUTPUT

![image](https://github.com/SGokul2005/Windows-basic-commands-batchscript/assets/147121825/a5a531ab-f05b-4aac-b9d3-47e3b2d95683)




# RESULT:
The commands/batch files are executed successfully.

