### What its?

1. `.git` folders
2. Git Errors
3. What is a diference bettwen `annotated tag` and `lighweight tag`
4. What is a diference bettwen `git checkout` and `git switch`
5. What is a diference bettwen `git merge` and `git rebase` ( R: Project History )

### How to do

1. How to install git.
2. How to configure git.
3. How to start with git
4. How to ignoring irrelevant content
5. How to clone a repository and save a file modification and push in remote repository.
6. How to do a CRUD with a commit.
7. How to change a file state.
8. How to work with git flow.
9. How to use branch list patterns.
10. How to resolve merge conflits.

- How to install git.
    
    ```docker
    sudo apt-get install git   -> Linux
    ```
    

- How to configure git.
    
    ```docker
    git config -l || cat .git/config       -> Show currently repository configurations.
    cat ~/.gitconfig                       -> Show global file config. Use Vim editor
    git config global <flag> <value>       -> Set Global configs
    ```
    

- How to start with git
    
    ```docker
    git init <new_folder_name>           -> Start git in local repository.
    git remote origin <url>              -> link local repository to remote repository.
    git branch -M main                   -> Create the main branch.
    git add . || git add <file_name>     -> Traked files in local respository.
    git commit -m "<message"             -> Save changes with a message tag.
    git push origin main                 -> Upload files to remote repository.
    ```
    

### Notes

`sudo apt-get install git`

`git config --global user.name <user_name>`

`git config --global user.email <user.email>`

`git log --online`

`git log -p`

`git log -- <filename>`

`git log --grg --decorate --online`

`git checkout -b <new_branch>`

`git branch --list`

`git branch -D <branch_name>`  

`git commmit -a -m "<message>"`

`git commit -am "<message>"`

`git status -s`

```jsx
??      -> untracked ( to add in staging area )
A       -> added ( to commit )
empty   -> working tree clean
```

 

`git rm`

```jsx
git rm -f         -> Force Delete a file on directory ( if status === added )
git rm            -> Delete a file on directory ( if status === commited )
git rm --cached   -> Delete a file on git index but leave in directory
```

`git tag`

```jsx
git tag                                -> List tags.
git tag -a <tag_name> -m "<message>"   -> Create a tag .
git show <tag_name>                    -> Show tag information.
git tag -d <tag_name>                  -> Delete tag.
main git-tag                           -> Local documentation for the git tag command.
```

`git branch` and `git checkout`

```jsx
git branch -la "<pattern>"         -> List All branchs ( pattern: optional )
git checkout -b <branch_name>      -> Create a new branch and swtich for this.
git checkout <branch_name>         -> Switch branch.
git branch -M <branch_name>        -> Move/Rename branch.
git branch -D <branch_name>        -> Delete branch ( Switch branch required )
git -t                             -> Substituto do --set-upstream
git branch --contains <commit>     -> List branches which contain the specified commit
git branch --no-contains <commit>  -> List branches which no contain the specified commit
main git-branch                    -> Local documentation for the git tag command.
main git-checkout                  -> Local documentation for the git tag command.
```

`git merge` and `git rebase`

```jsx

```

`git revert <commit>`

`git diff`