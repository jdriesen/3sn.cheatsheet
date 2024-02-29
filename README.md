# Git &amp; Github Cheat Sheet by 3SN
3sn.cheatsheet

## Youtube resources

[The very basics](https://www.youtube.com/watch?v=mJ-qvsxPHpY)   
[A bit more advanced, though still very understandable](https://www.youtube.com/watch?v=tRZGeaHPoaw)

## Defining your name and email
```csharp
/* These settings will be used in ALL your repo's. */
/* Has to be done only once                        */ 
git config --global user.name  "Your Name"
git config --global user.email "Your email"
```

## Initialising your LOCAL repo
```csharp
/* Has to be done only once PER PROJECT            */ 

/* 
=== Remark ====
I strongly recommend to:   
1. Create your project on Github 
2. and clone it locally 
3. Merge the .git folder and the readme file with your local files..
*/

// Other solution:
git init // In local Project Folder.
```

## CREATE / DEFINE Aliases

```csharp
git config --global alias.<alias_name> "<git_command>"

// Example
git config --global alias.co "checkout"
```

## Overview ALIASES
All ALIASES are stored in a local file, named **.gitconfig**.   
On a Windows system, this file is located in the folder **C:\Users\\<user_name>\\.gitconfig**


## COMMON aliases
```csharp 
// Status
// -- git status
  git stat  
```

## BRANCHES aliases
```csharp 
// 1. CREATE a new branch with the specified name. 
//   -- git branch <branch-name>
  git brc <branch-name>

// 2. CHECK OUT / SWITCH TO a specified branch.
//   -- git checkout <branch-name>
git bro <branch-name>       

// 1 & 2 CREATE & CHECK OUT / SWITCH TO a specified branch.
//   -- git checkout -b <new-branch-name>
git brco <new-branch-name> 

// MERGE the specified branch into the CURRENT branch.
//   -- git merge <specific-branch-name>
git brm <specific-branch-name>

// DELETE the specified branch.
//   -- git branch -d <branch-name>
git brd <branch-name>


// 3. LIST all LOCAL branches in the repository
//    -- git branch
git brll   

// 4. LIST all REMOTE branches.
//    -- git branch -r
git brlr

// 3 & 4. LIST all REMOTE branches.
//    -- git branch -a
git brla
```



## STAGING Related
```csharp 
// 1. Add All Files to staging 
//   --  git add . or git add –all
git adda                     
  
// 2. Commit with message 
//   --  git commit -m “<message>” or git commit –message “<message>”
git com “<message>”          

// 1 & 2. Add all Files to staging and Commit with message.... All in One .:. BETTER .:.  
//   -- git commit -a -m “<message>” or git commit –all –message “<message>”
git coma “<message>”  
```








* brc : git branch .:. Lists all branches in the repository.
```csharp 
  git br // Lists all branches in the repository
  git br branch_name // 
  ```



* brc for **checkout**: Create a branch   
  ```csharp 
  git out branch_name
  ```


* out for **checkout**: Switch branches or restore working tree files.   
  ```csharp 
  git out branch_name
  ```


* com for commit:   
Record changes to the repository.

* stat for status:   
Show the working tree status.

* bra for branch:   
List, create, or delete branches.

* log for log:   
Show commit logs.

* dif for diff:   
Show changes between commits, commit and working tree, etc.  

Using Shortcut Commands: After creating aliases, simply use them in place of the original 

