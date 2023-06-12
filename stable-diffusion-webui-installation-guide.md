# Install and run Stable Diffusion Web UI (Automatic1111)

   - [Install Stable Diffusion Web UI on Mac](#Install-Stable-Diffusion-Web-UI-on-Mac)
   - [Run Stable Diffusion Web UI on Mac](#Run-Stable-Diffusion-Web-UI-on-Mac)
   - [End Stable Diffusion Web UI on Mac](#End-Stable-Diffusion-Web-UI-on-Mac)
   - [Update Stable Diffusion Web UI on Mac](#Update-Stable-Diffusion-Web-UI-on-Mac)
  - [Installation Guides for other Operating Systems](#Installation-Guides-for-other-Operating-Systems)



## Install Stable Diffusion Web UI on Mac

###  Step 1 - Install Homebrew

To install [Homebrew](https://brew.sh/index) on a Mac, you can follow these steps:

1. Open the Terminal application. You can find it in the Applications folder, under the Utilities subfolder, or you can use Spotlight search (press Command + Space and type "Terminal").

2. In the Terminal, paste the following command and press Enter:

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

This command will download and run the Homebrew installation script.

3. The script will prompt you to continue with the installation. It will ask for your password, as it needs administrator privileges to install Homebrew. Type your password (you won't see it as you type) and press Enter.

4. The installation process may take a few minutes. It will download and install the necessary files and dependencies.

5. Once the installation is complete, you should see a message indicating that Homebrew has been successfully installed.


After installing Homebrew on your Mac, you may need to adjust your PATH environment variable to ensure that Homebrew commands are recognized and accessible from any directory in the Terminal. Here's how you can do it:

1. Open the Terminal application.

2. Run the following command to open the Bash configuration file in a text editor:

   ```
   open ~/.bash_profile
   ```

   If you are using a different shell, such as Zsh, you may need to open a different configuration file. For Zsh, you can use `~/.zshrc` instead of `~/.bash_profile`.

3. The configuration file will open in your default text editor. Add the following line at the end of the file:

   ```
   export PATH="/usr/local/bin:$PATH"
   ```

   This line adds the Homebrew binary directory to the beginning of your PATH variable, ensuring that Homebrew commands take precedence over system commands with the same name.

4. Save the file and close the text editor.

5. In the Terminal, run the following command to apply the changes to your current session:

   ```
   source ~/.bash_profile
   ```

   If you are using Zsh or a different shell, use `source ~/.zshrc` instead.

Now your PATH variable is updated to include the Homebrew binary directory, and you should be able to use Homebrew commands from any directory in the Terminal. You can verify this by running `brew doctor` or any other Homebrew command to see if it executes successfully.

Congratulations! You have successfully installed Homebrew on your Mac. You can now use Homebrew to install various packages and software on your machine.

### Step 2 - Use Homebrew to Install Required Applications

Run the the following command in your terminal app:

 ```
 brew install cmake protobuf rust python@3.10 git wget
  ```

This instructs Homebrew to download and install the following packages on your Mac:

1. `cmake`: CMake is an open-source, cross-platform build system that helps in managing the build process of software projects. It provides a platform-independent way to configure, build, and test software.

2. `protobuf`: Protocol Buffers is a language-agnostic serialization format developed by Google. It allows you to define the structure of your data using a simple language and generate code for various programming languages to serialize, deserialize, and manipulate the data efficiently.

3. `rust`: Rust is a systems programming language known for its focus on memory safety, concurrency, and performance. It aims to provide a reliable and efficient way to develop low-level software, such as operating systems, device drivers, and embedded systems.

4. `python@3.10`: This installs Python version 3.10 using Homebrew. Python is a popular programming language known for its simplicity and versatility. The version number specifies the specific version of Python you want to install. It's worth noting that the version may change over time, and you can replace `3.10` with a different version if desired.

5. `git`: Git is a widely used version control system that helps you track changes in your source code and collaborate with others efficiently. It allows multiple developers to work on a project simultaneously, manage different versions of the code, and merge changes seamlessly.

6. `wget`: Wget is a command-line utility for downloading files from the web. It supports various protocols, including HTTP, HTTPS, and FTP, and provides features like recursive downloading, resuming interrupted downloads, and downloading files in the background.

### Step 3 - Install Stable Diffusion Web UI

Stable Diffusion Web UI can be found in a GitHub repository called [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui). To install it locally on your mac, you must clone this GitHub repository by following these steps:
To clone the repository "stable-diffusion-webui" on your Mac, you can follow these steps:

1. Open the Terminal application on your Mac.

2. Navigate to the directory where you want to clone the repository. You can change directories using the `cd` command. For example, to navigate to your "Documents" folder, you can use the following command:

   ```
   cd Documents
   ```

3. Once you are in the desired directory, run the following command to clone the repository:

   ```
   git clone https://github.com/AUTOMATIC1111/stable-diffusion-webui
   ```

   This command instructs Git to clone the repository from the specified URL.

4. Git will start cloning the repository to your current directory. The progress will be displayed in the Terminal, and once it's complete, you will have a local copy of the repository on your Mac.

Now you have successfully cloned the "stable-diffusion-webui" repository to your Mac. You can navigate to the cloned repository using the `cd` command and explore the files and folders within it.

### Download the Model

1. Download Stable Diffusion model version 1.5 by clicking on [this link](https://huggingface.co/runwayml/stable-diffusion-v1-5/resolve/main/v1-5-pruned-emaonly.ckpt)

2. Place the downloaded file into the following folder of the GitHub repository you have cloned in step 3

> stable-diffusion-webui/models/Stable-diffusion

Congratulations! You have successfully installed Stable Diffusion Web UI on your mac and you're now ready to start generating images.

## Run Stable Diffusion Web UI on Mac

1. Open the Terminal application on your Mac.

2. Navigate to the directory where you want repository was cloned. You can change directories using the `cd` command. For example, to navigate to your "stable-diffusion-webui" folder, you can use the following command:

   ```
   cd stable-diffusion-webui
   ```

3. Once you are in the desired directory, run the following command to start Stable Diffusion Web UI:

   ```
   ./webui.sh
   ```

   This will create a Python virtual environment in which Stable Diffussion can be started within a browser. The link to access this virtual environment will be provided to you within the terminal app.

4. Copy the URL provided to you in the terminal app and paste it in a browser. Pythom will always generate the same URL. You can therefore save it as a bookmark in your browser. However, it will only run if the virtual environment is active.

## End Stable Diffusion Web UI on Mac

Closing the browser window for Stable Diffusion Web UI is not sufficient. The virtual environment will keep running and consume resources. You will have to terminate the virtual environment session by following these steps:

1. Go back to the Terminal application on your Mac (which should still be running).

2. Press the following key combination on your keyboard:

   ```
   CONTROL + C
   ```
This will interrupt the viertual environment session.

## Update Stable Diffusion Web UI on Mac

To update Stable Diffusion Web UI, you need to pull the latest changes from GitHub repository [AUTOMATIC1111/stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui):

1. Open the Terminal application on your Mac.

2. Navigate to the directory where you want repository was cloned. You can change directories using the `cd` command. For example, to navigate to your "stable-diffusion-webui" folder, you can use the following command:

   ```
   cd stable-diffusion-webui
   ```

3. Once you are in the desired directory, run the following command to start Stable Diffusion Web UI:

   ```
   git pull
   ```

   This will update your local copy of Stable Diffusion Web UI with the latest changes.

## Installation Guides for other Operating Systems

- [Installation guide for Windows](https://github.com/AUTOMATIC1111/stable-diffusion-webui#automatic-installation-on-windows)
- [Installation guide for Linux](https://github.com/AUTOMATIC1111/stable-diffusion-webui#automatic-installation-on-linux)

