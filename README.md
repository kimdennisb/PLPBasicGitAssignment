# PLPBasicGitAssignment

### 1. **Initialize a Local Git Repository**
- **Command**:
  ```bash
  git init
  ```

This command creates a new Git repository in your current directory.

### 2. **Connect Local Repository to Remote Origin**
To connect your local repository to the remote repository
- **Command**:
  ```bash
  git remote add origin <repository-url>
  ```
- Example:
  ```bash
  git remote add origin https://github.com/username/repository.git
  ```

This command links your local repository to the remote repository.

### 3. **Verify Remote Connection**
You can verify that the remote connection was added successfully by running:
- **Command**:
  ```bash
  git remote -v
  ```

You should see something like:
```
origin  https://github.com/username/repository.git (fetch)
origin  https://github.com/username/repository.git (push)
```

### 4. **Add Files to Local Repository**
To track files in your local repository:
- **Command**:
  ```bash
  git add <file-name>
  ```
- To add all files in the repository:
  ```bash
  git add hello.txt
  ```

### 5. **Commit Changes to Local Repository**
After adding files, commit the changes:
- **Command**:
  ```bash
  git commit -m "Initial commit"
  ```

This commits the changes to your local Git history.

### 6. **Push Changes to the Remote Repository**
Now that your local repository is connected to the remote origin and the files are committed, push the changes to the remote repository:
- **Command**:
  ```bash
  git push -u origin <branch-name>
  ```
- For example, to push to the `main` branch:
  ```bash
  git push -u origin main
  ```

The `-u` flag sets the upstream branch, linking your local branch with the remote one so that subsequent pushes can be done with just `git push`.

### 7. **Pull Changes from Remote**
If you want to fetch and merge any changes from the remote repository, use:
- **Command**:
  ```bash
  git pull origin <branch-name>
  ```