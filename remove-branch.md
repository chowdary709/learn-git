To remove branches in your local Git repository on macOS (or any other operating system), you can use the `git branch -d` or `git branch -D` command. Here's how you can do it:

### 1. List All Branches
First, list all branches to identify which ones you want to delete:

```sh
git branch
```

This command will show a list of all local branches, with the current branch highlighted by an asterisk (*).

### 2. Delete a Local Branch
#### If the Branch Has Been Merged
If the branch you want to delete has been merged into another branch (typically `main` or `master`), you can delete it using the `-d` option:

```sh
git branch -d branch-name
```

Replace `branch-name` with the name of the branch you want to delete.

#### If the Branch Has Not Been Merged
If the branch has not been merged and you still want to delete it, use the `-D` option to force delete it:

```sh
git branch -D branch-name
```

Replace `branch-name` with the name of the branch you want to delete.

### Example Workflow

1. List all branches:

    ```sh
    git branch
    ```

2. Delete a merged branch (e.g., `feature-1`):

    ```sh
    git branch -d feature-1
    ```

3. Force delete an unmerged branch (e.g., `feature-1`):

    ```sh
    git branch -D feature-1
    ```

### Note
- **Ensure you are not on the branch you are trying to delete**. You cannot delete the branch you are currently on. Switch to another branch, such as `main`, before deleting:

    ```sh
    git checkout main
    ```

- **Be cautious with the `-D` option**: It will delete the branch regardless of its merge status, potentially leading to loss of work if the branch has unmerged changes.

By following these steps, you can effectively manage and delete branches in your local Git repository on macOS.