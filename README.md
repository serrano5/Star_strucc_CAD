# Star_strucc_CAD
## repo for storing and tracking CAD files and ANSYS files.

## Repo Structure:  
Keep completed/in progress assemblies in the assemblies folder. Keep all dependencies like parts and subassemblies in the dependencies folder. After cloning, add any existing assemblies and dependencies to your local copy of the repo, open all assemblies that need dependencies rerouted, and when prompted point SolidWorks to where those files are stored in the dependencies folder. Make sure to save. 

Keep ANSYS projects stored in subfolders in the ANSYS directory.  

## Command line Setup 
(idk how to use Git Desktop but should be an easier setup than command line):  
-navigate to where you want the files stored  
`git clone https://github.com/jhensley99/Star_strucc_CAD.git`
-move lcoally stored files into the proper locations and update SolidWorks and ANSYS file pointer  

    git add .
    git commit -m "description"
    git push origin main

A login window may appear. Use a non-MIT Github account! The MIT Enterprise server wouldn't allow me to use https, and Git LFS currently does not support SSH, so a github.com account is required. Once you login on the popup window (popup may not appear. Don't worry about it if it doesn't) you will be prompeted to sign in on the command line. Github no longer supports password logins, so you will need to generate a public access token and use that as the password. Info on how to do that can be found here: https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token  
I recommend setting the access token to last until the end of the semester so you won't have to worry about it again. After logging in once, you shouldn't be prompted to login again until the token expires. You should now be able to push to/pull from the repo. 

## Git LFS
Git large file system is being used to track changes in Solidworks and ANSYS files. Install it using `git install lfs` or by downloading and running it from https://git-lfs.github.com/. Tracked file extensoins can be found in .gitattributes. If there is a file type you would like tracked by LFS, add it by `git lfs track *.file_extension` then push. Changes should be reflected in .gitattributes. 
