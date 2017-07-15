
# Git Large File storage easiest steps

Git is distributed version control system and there is limit of file size to add in public repository. GitHub file size limit to 100MB so if you would like to add larger file then 100MB follow below easiest steps.


### GitHub Large file Storage easiest steps: (Mac)

### Step 1:

@Terminal 
Install Git-lfs:

      $ brew install git-lfs
        
Need to install once only

### Step 2:

@project directory /File folder
Initialized empty Git repository:

      $ git Init

### Step 3:

Git LFS initialized:

      $ git lfs install 
    
This step is in particular file folder to initialized/ hook git lfs in folder.

output:
-MacBook-Pro:large_file $ git lfs install
      Updated git hooks.
      Git LFS initialized.

### Step 4:

Select all types files to track and handled by git lfs

      $ git lfs track "*.csv"
      $ git lfs track "*.db"
      $ git lfs track "*.osm"
      $ git lfs track "*.psd"
      $ git lfs track "*.gif"

Git lfs track pattern of all files .extension
track with "*.extension" track all files with that extension.

### Step 5:

      $ git add .gitattributes

this add all track attributes in this file

you can check which file git lfs tracking by 
      
      $ git lfs track

Listing tracked patterns
    *.osm (.gitattributes)
    *.db (.gitattributes)
    *.csv (.gitattributes)

### Step 6:

Start adding and commit files as normally git add file

      $ git add fun_nodes.csv

git commit -m "initial fun large file commit"

### Step 7:

To push file in git repository

      $ git lfs push origin master

### Step 8:

      $ git push 

Note: Now you refresh github repository and you can see all your large file and for small file you can do as normal process.

