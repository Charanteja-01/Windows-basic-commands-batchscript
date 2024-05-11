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
~~~
mkdir %userprofile%\Desktop\MyLab
~~~

![329449798-398612b3-9655-420e-a9c9-f200a24d5232](https://github.com/Charanteja-01/Windows-basic-commands-batchscript/assets/145693038/c9035e61-534a-4873-8678-81ca12c6fe98)

## COMMAND AND OUTPUT


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
![329451087-56ead55b-3ebc-457a-9b66-9e794536ea8d](https://github.com/Charanteja-01/Windows-basic-commands-batchscript/assets/145693038/63cbc4cb-5265-4c2a-85d7-fba1d32cd1eb)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
~~~
cd %userprofile%\Desktop\MyLab
~~~

![329449993-d1900a0b-4c3c-4770-bafa-39161e0a2c1c](https://github.com/Charanteja-01/Windows-basic-commands-batchscript/assets/145693038/6365900d-147f-4943-9068-27c7ab7829af)

![329450045-bffe5243-b728-440c-af14-be8e5105bab9](https://github.com/Charanteja-01/Windows-basic-commands-batchscript/assets/145693038/a3a28633-c3df-4062-af63-ce9cc9eaf1a6)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

~~~
dir %userprofile%\Desktop\MyLab
~~~

![329450216-ed4e8f45-9c2b-4c9a-9220-63bd3cfe0baa](https://github.com/Charanteja-01/Windows-basic-commands-batchscript/assets/145693038/48d0ccc1-06d3-4cc5-b0d2-b1096023f8d0)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
~~~
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
~~~

![329450372-a71f24b7-e9c4-40c6-a824-55f3466b4095](https://github.com/Charanteja-01/Windows-basic-commands-batchscript/assets/145693038/ee05b5f1-779f-425b-ba23-29aa005f77a4)
![329450418-6b368260-d83c-4bb4-bdb8-8fd0601a9dd7](https://github.com/Charanteja-01/Windows-basic-commands-batchscript/assets/145693038/638aa857-f7bd-4c36-aca2-199fcbd5781b)



## COMMAND AND OUTPUT
~~~
mv Myfile.txt %userprofile%\Documents
~~~

![329450533-49dd374a-73a4-47f1-946f-86963b81a5b6](https://github.com/Charanteja-01/Windows-basic-commands-batchscript/assets/145693038/5d9c6071-f116-49fd-ab6a-3a47b88c76a4)

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
![329450771-e6f191cf-508d-4d3e-91da-9b9c27b9ab4c](https://github.com/Charanteja-01/Windows-basic-commands-batchscript/assets/145693038/ef79a10e-312a-49a9-94da-5688880d053c)










# RESULT:
The commands/batch files are executed successfully.

