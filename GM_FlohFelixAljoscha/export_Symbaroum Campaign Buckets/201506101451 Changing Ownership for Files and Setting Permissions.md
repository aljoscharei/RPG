# Changing Ownership for Files and Setting Permissions
 [[Computer]] [[Apple]] 
---



_Every Monday, we'll show you how to do something new and simple with Apple's built-in command line application. You don't need any fancy software, or a knowledge of coding to do any of these. All you need is a keyboard to type 'em out!
_
When copying a file between one system and another, occasionally both the permissions and owner for the files will be incorrect. You may need to change the owner of the file because the file is unable to be edited by the user due to permissions issues. While you could mess with the Finder’s “Get Info” panel to make these changes, there’s a better, and more simple way to change a large group of files at the same time. We’ll rely on the “chown” command to change the owner of a specified group of files, right from the command line.

### What is File Ownership?

File ownership simply means the files that were created by a particular user. These files are therefore “owned” by that user. Users who do not own the files cannot edit them unless that user has super user privileges (and can run the “sudo” modifier on the edit command), or that user belongs to the same group as the file is assigned to.

### Changing one File

[![unknown_filename.png](./resources/201506101451_Changing_Ownership_for_Files_and_Setting_Permissions.resources/unknown_filename.png)](http://www.maclife.com/files/u12635/fileownership.png)

If you only wish to change the owner of a single file, then we’ll use a specific command that is different from the recursive command for directories. Before you begin, however, you’ll need to know the shortname of the user you will be assigning the files to. This will be the name of the user’s home directory in the Finder. 
Once you have this bit of information, you can issue the following command:

sudo chown -v username file

Replace “username” with the shortname of the user who will be assigned the files, and replace “file” with the path and name of the file to be assigned. Because we used the -v flag (for verbose mode), you will see the file and what changed printed to the command line.

### Changing a group of Files

[![unknown_filename.1.png](./resources/201506101451_Changing_Ownership_for_Files_and_Setting_Permissions.resources/unknown_filename.1.png)](http://www.maclife.com/files/u12635/dirownership.png)

You may need to change ownership for a directory and all of the files and subdirectories contained within. You can easily do this by adding the recursive flag to the command, like so:

`sudo chown -Rv username directory` 

Replace the “username” placeholder above with the shortname of the user who will be assigned the files, and replace “directory” with the path and name of the directory whose contents will be assigned to the user. Again, we used the -v flag in addition to the -R flag. This means that the command will output the files changed to the screen, so you can see exactly what happened.

Setting read and Write:

`chmod -R +rw html/`

---

_Created at 20150610._
_Last updated at 20150610._



