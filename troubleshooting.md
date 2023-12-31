# Troubleshooting Guide

## Common Issues When Cloning the Repository

### 1. **Error: "fatal: destination path 'repository-name' already exists and is not an empty directory."**

If you come across this error, it suggests that there exists a folder with the same name as the repository you are attempting to clone. This folder might be hidden, and as a result, you won't be able to locate it in your Finder (or File Explorer on Windows).

To address this, you can attempt using the following command, allowing you to designate a new name for the cloned repository:

```bash
git clone <url-link> <new-repo-name>
```

For example, in your situation, you can use:

```bash
git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui.git stable-diffusion
```

This command will clone the repository into a folder named "stable-diffusion," mitigating the error associated with the pre-existing folder. 

If the issue persists, ensure to inspect your system for hidden folders, as there could be a directory not immediately visible.

#### [Optional] Check for Hidden Directories

Make sure you are in the correct directory where you want to clone the repository. Use the `cd` command to navigate to the desired directory:

```bash
cd /path/to/desired/directory
```

Use the `ls -a` command to list all files, including hidden ones, in the current directory. Look for a '.git' directory:

```bash
ls -a
```

If you find a '.git' directory, it means there is an existing Git repository. You can choose to delete it if you want to start fresh:

```bash
rm -rf .git
```
