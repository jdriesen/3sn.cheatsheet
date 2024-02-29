## Git &amp; Github Cheat Sheet by 3SN
3sn.cheatsheet   
All ALIASES are stored in a local file, named **.gitconfig**.   
On a Windows system, this file is located in the folder **C:\Users\\<user_name>\\.gitconfig**

### Youtube resources

[The very basics](https://www.youtube.com/watch?v=mJ-qvsxPHpY)   
[A bit more advanced, though still very understandable](https://www.youtube.com/watch?v=tRZGeaHPoaw)

```csharp
// Defining your name and email

/* These settings will be used in ALL your repo's. */
/* Has to be done only once                        */ 
git config --global user.name  "Your Name"
git config --global user.email "Your email"
```

### Initialising your LOCAL repo
```csharp
/* Has to be done only once PER PROJECT          
=== Remark ====
I strongly recommend to:   
1. Create your project on Github 
2. and clone it locally 
3. Merge the .git folder and the readme file with your local files.. */

// Other solution:
git init // In local Project Folder.
```

```csharp
// CREATE / DEFINE Aliases
git config --global alias.<alias_name> "<git_command>"

// Example
git config --global alias.co "checkout"
```

### COMMON aliases
```csharp 
// Status .:. Current situation
git stat // -- git status

// Log in 1 line
git lo1 // -- log --oneline

// Tree show log in tree format
git tree // -- log --oneline --graph --decorate --all
```

## BRANCHES ( bra_ ) aliases
```csharp 
// 1. BRANCH CREATE .:. Creates a branch with a specified name. 
git brac <new_branch_name> // -- git branch <branch-name>

// 2. BRANCH checkOUT / SWITCH TO a specified branch.
git brao <branch_name> // -- git checkout <branch-name>       

// 1 & 2 BRANCH CREATE & check OUT / SWITCH TO a specified branch.
git braco <new_branch_name> //   -- git checkout -b <new-branch-name> 

// BRANCH MERGE the specified branch into the CURRENT branch.
git bram  <specific_branch_name> //   -- git merge --nof <specific-branch-name>

// BRANCH DELETE the specified branch.
git brad <branch_name> //   -- git branch -d <branch-name>

// 3. BRANCH (LIST) LOCAL branches in the repository
git bral OR git brall //    -- git branch   

// 4. BRANCH (LIST) REMOTE branches.
git brar OR git bralr //    -- git branch -r

// 3 & 4. BRANCH (LIST) ALL branches.
git braa OR git brla //    -- git branch -a
```

## STAGING ( sta_ ) Aliases
```csharp 
// 0. STAGE (one) FILE to staging 
git staf <filename>  //   --  git add <filename>

// 1. STAGE ALL Files to staging 
git staa    // --  git add . OR git add –all                    
  
// 2. STAGE COMMIT with message 
git stacom “<msg>” //   --  git commit -m “<msg>” OR git commit –message “<msg>”          

// 1 & 2. STAGE COMMIT ALL .:. Add all Files to staging and Commit with message.  
git stacoma “<msg>” //   -- git commit -am “<msg>” OR git commit –all –message “<msg>”  

// STAGE DELETE One File from staging (but keep changes) 
$ git stad <filename> //   --  git reset HEAD <filename>

// STAGE DELETE ALL Files from staging (but keep changes)
$ git stada  //   --  git reset HEAD
```

## FREQUENTLY Used
```csharp 

// Create Branch 
git braco <branchname>

/* ------------------------ */
/* --- Solved Your BUG ---- */
/* ------------------------ */

// Commit All your files to staging with a message
git stacoma <msg>

// checkout MAIN branch 
git brao main

// Merge branch into main
git bram <branchname>
```


## REMOTE Aliases
```csharp 
// PULL / GET all files from Github 
git pull //   --  git pull
  
// PUSH / SEND all Changes TO Github 
git push //   --  git push          
```
