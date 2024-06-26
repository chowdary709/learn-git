Sure! The commands you provided are mostly correct, but they need a slight adjustment to form a proper sequence. Here is the correct sequence of commands:

1. **Add all changes**: Stage all the changes in the current directory.
   ```sh
   git add .
   ```

2. **Commit the changes**: Commit the staged changes with a message.
   ```sh
   git commit -m "commit-1 from feature-1"
   ```

3. **Push the changes**: Push the committed changes to the remote repository on the `feature-1` branch.
   ```sh
   git push origin feature-1
   ```

For convenience, you can run these commands in a single line separated by semicolons:

```sh
git add .; git commit -m "commit-1 from feature-1"; git push origin feature-1
```

### Complete Workflow

Assuming you are already on the `feature-1` branch, the complete workflow would look like this:

1. **Open Terminal** and navigate to your repository:
   ```sh
   cd /path/to/your/repository
   ```

2. **Create or switch to the feature branch** (if not already on it):
   ```sh
   git checkout -b feature-1
   ```

3. **Make your changes**: Edit your files as needed.

4. **Add, commit, and push your changes**:
   ```sh
   git add .; git commit -m "commit-1 from feature-1"; git push origin feature-1
   ```

This will stage all the changes, commit them with the specified message, and push the changes to the `feature-1` branch on the remote repository.

Feel free to ask if you have any more questions or need further clarification!