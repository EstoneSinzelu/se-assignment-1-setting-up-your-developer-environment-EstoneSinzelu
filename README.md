[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/vbnbTt5m)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15252260&assignment_repo_type=AssignmentRepo)
# Dev_Setup
Setup Development Environment
#The images are in the links
#Assignment: Setting Up Your Developer Environment

#Objective:
This assignment aims to familiarize you with the tools and configurations necessary to set up an efficient developer environment for software engineering projects. Completing this assignment will give you the skills required to set up a robust and productive workspace conducive to coding, debugging, version control, and collaboration.

#Tasks:

1. Select Your Operating System (OS):
   Choose an operating system that best suits your preferences and project requirements. Download and Install Windows 11. https://www.microsoft.com/software-download/windows11
Getting Windows 11 on your 64-bit machine involves checking compatibility, creating a bootable USB drive, and following the installation process.

**First things first - Is your PC okay for Windows 11?**

* Processor: 64-bit with 2 cores and at least 1 GHz speed
* RAM: 4 GB or more
* Storage: At least 64GB free
* System firmware: Must be UEFI and support Secure Boot
* TPM: Trusted Platform Module version 2.0 required
* Graphics: DirectX 12 or later with WDDM 2.0 driver
* Display: High-definition (720p) with at least 8 bits per color channel

There's a free PC Health Check app by Microsoft that can check your system for you.

**Ready to install? Let's make a bootable USB drive.**

1. Download the Installation Assistant tool from the Microsoft website.
2. Run the tool and choose to create installation media for another PC.
3. Pick your language, Windows 11 edition (Home or Pro), and 64-bit architecture.
4. Select a USB drive with at least 8GB of space (be warned, this will erase everything on the drive so back up anything important first!)
5. The tool will download Windows 11 and create the bootable USB drive. This might take a while.

**Now to get Windows 11 on your machine.**

1. Back up any important files, just in case.
2. Restart your computer and press a specific key (like Esc, Delete, F2, F10, or F12) to enter the BIOS or UEFI settings menu (check your motherboard manual for the exact key).
3. Once in BIOS/UEFI, find the boot priority section and set your USB drive to boot first. Save changes and exit.
4. Your computer should boot from the USB drive and start the Windows 11 setup process. Follow the on-screen instructions.
5. You'll be asked about language, keyboard layout, and installation type (Upgrade or Custom). Upgrade keeps your existing files and settings, while Custom does a clean install (erasing everything).
6. Follow the prompts to create a user account, connect to the internet, and configure Windows 11 settings.

**All done!** Your computer will restart, and you'll be up and running with Windows 11. Windows Update might download and install additional drivers and updates.

**Tips:**

* Keep the bootable USB drive for future reinstalls.
* Microsoft has more detailed guides online if you get stuck.
* You can't include screenshots here, but searching online can help you find images for steps like navigating the BIOS/UEFI settings (which will vary depending on your motherboard).
2. Install a Text Editor or Integrated Development Environment (IDE):
   Select and install a text editor or IDE suitable for your programming languages and workflow. Download and Install Visual Studio Code. https://code.visualstudio.com/Download
   Here's how to download and install Visual Studio Code (VS Code) on your Windows 11 64-bit system:

**Downloading VS Code:**

1. Go to the official VS Code download page: [download visual studio code ON code.visualstudio.com]
2. Under the "Download for Windows" section, you'll see two options:
    * **User Installer (x64)**: This is the recommended option for most users.
    * **System Installer (x64)**: This option allows you to install VS Code for all users on your system. Choose this if you want multiple users to be able to access VS Code.

**Installing VS Code:**

1. Click on the download button for your preferred installer type (User or System).
2. The download will start. Once it's finished, locate the downloaded file (usually in your Downloads folder) and double-click it to run the installer.
3. The installation wizard will open. Here are some recommended options during installation:
    * **Leave the default installation location** (usually `C:\Users\{username}\AppData\Local\Programs\Microsoft VS Code`).
    * **Check the box to "Add VS Code to PATH"** if you want to be able to launch VS Code from any command prompt or terminal window.
    * You can customize other options based on your preferences.
4. Click "Install" to begin the installation process.
5. Once the installation is complete, you can launch VS Code by searching for it in the Start menu or taskbar search.

**Additional Tips:**

* You can check the official VS Code documentation for Windows for more detailed information on the installation process: [https://code.visualstudio.com/docs/setup/windows](https://code.visualstudio.com/docs/setup/windows)
* There's also a helpful video guide on YouTube that walks you through the installation steps visually: [how to install visual studio code on windows 10 11] (Note: this video link is for reference only, following the steps mentioned above is recommended)
3. Set Up Version Control System:
   Install Git and configure it on your local machine. Create a GitHub account for hosting your repositories. Initialize a Git repository for your project and make your first commit. https://github.com

**1. Install Git:**

* Visit the official Git downloads page: [https://www.git-scm.com/downloads](https://www.git-scm.com/downloads)
* Download the installer for your operating system (Windows, macOS, Linux).
* Run the installer and follow the on-screen instructions.

**2. Configure Git (Optional):**

* Open a terminal window (Command Prompt on Windows, Terminal on macOS/Linux).
* Type the following command to check if Git is installed correctly:

```
git --version
```

* This should display the installed Git version.

* You can optionally configure your username and email address for Git commits using:

```
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

**3. Create a GitHub Account:**

* Go to GitHub: [invalid URL removed]
* Click "Sign Up" and create a free account.

**4. Initialize a Git Repository:**

* Open a terminal window and navigate to your project directory using the `cd` command.
* Initialize a new Git repository in your project directory by running:

```
git init
```

This creates a hidden folder called `.git` that stores the version control information.

**5. Create Your First Commit:**

* Make some changes to your project files (e.g., write some code, edit a document).
* Use the `git status` command to see which files have been modified.
* Use the `git add` command to stage the changes you want to include in your commit. For example, to add all modified files:

```
git add .
```

* You can add specific files by mentioning their names after `git add`.
* Enter a descriptive commit message using `git commit -m "Your message here"`. This message explains what changes you made.

**6. Push to GitHub (Remote Repository):**

* Create a new repository on GitHub for your project (if you haven't already).
* In your terminal, run the following commands to link your local repository to the remote repository on GitHub (replace `<username>` and `<repository-name>` with your actual details):

```
git remote add origin git@github.com:<username>/<repository-name>.git
git push -u origin main
```

**Explanation:**

* `git remote add origin ...` creates a named remote ("origin") that points to your GitHub repository URL.
* `git push -u origin main` pushes your local changes (the `main` branch) to the remote repository on GitHub for the first time. The `-u` flag sets the "upstream" branch, simplifying future pushes.

**Additional Notes:**

* You can find detailed Git commands and explanations in the official Git documentation: [https://git-scm.com/book](https://git-scm.com/book)
* GitHub provides excellent tutorials and guides to get you started with version control: [https://www.atlassian.com/git/tutorials](https://www.atlassian.com/git/tutorials)
4. Install Necessary Programming Languages and Runtimes:
  Instal Python from http://wwww.python.org programming language required for your project and install their respective compilers, interpreters, or runtimes. Ensure you have the necessary tools to build and execute your code.
**1. Download the Python Installer:**

- Head over to the official Python website: [https://www.python.org/downloads/](https://www.python.org/downloads/)
- Locate the download section based on your operating system (Windows, macOS, or Linux).
- Download the appropriate installer for your system (typically a `.msi` for Windows, a `.pkg` for macOS, or a `.gz` or `.bz2` archive for Linux).

**2. Install Python (Windows):**

- Double-click the downloaded `.msi` installer.
- In the installation wizard, it's generally recommended to keep the default settings (which include adding Python to your system path). This allows you to run Python commands from any directory in your command prompt or terminal.
- Click "Install" and follow any on-screen instructions.

**2. Install Python (macOS):**

- Double-click the downloaded `.pkg` installer.
- Follow the on-screen prompts, which typically involve agreeing to the license terms and choosing an installation location.
- Python will be installed, and you should be good to go.

**2. Install Python (Linux):**

- The installation process for Linux varies depending on your distribution. Here are some common methods:

    - Using your package manager (recommended):
        - Open a terminal window.
        - Identify your package manager (e.g., `apt`, `yum`, `dnf`) using a command like `which apt` (if applicable).
        - Update your package lists:
            ```bash
            sudo apt update  # For Debian/Ubuntu-based systems
            sudo yum update   # For Red Hat-based systems
            ```
        - Install Python using your package manager:
            ```bash
            sudo apt install python3  # For Debian/Ubuntu-based systems
            sudo yum install python3  # For Red Hat-based systems
            ```
    - Downloading from source (advanced):
        - Visit the Python downloads page again and download the source code archive (`.gz` or `.bz2`).
        - Extract the archive.
        - Navigate to the extracted directory in your terminal.
        - Run the configuration script (e.g., `./configure`).
        - Build and install Python using `make` and `sudo make altinstall` (adjust commands as needed).

**3. Verify Installation:**

- Open a terminal or command prompt window.
- Type `python --version` (or `python3 --version` on Linux if multiple Python versions exist).
- If the installation was successful, you should see the installed Python version displayed.

**Congratulations! You now have Python and its runtime environment set up.**

**Additional Notes:**

- If you encounter issues during installation, refer to the official Python documentation for your operating system: [https://docs.python.org/3/download.html](https://docs.python.org/3/download.html)
- Consider using a virtual environment to manage different Python versions and their dependencies for specific projects: [https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/)
5. Install Package Managers:
   If applicable, install package managers like pip (Python).
## Installing pip (Python Package Manager)

**pip** is the most common package manager for Python. Here's how to install it depending on your operating system:
**Windows:**

1. **Check if pip is already installed:** Open a Command Prompt window and type `pip --version`. If pip is installed, you'll see the version number.
2. **Install Python (if not already installed):** Download and install the latest version of Python from [https://www.python.org/downloads/](https://www.python.org/downloads/). Make sure you check the option "Add Python to PATH" during installation. This will allow you to run pip commands from any directory in your Command Prompt.
3. **Verify pip installation:** Open a new Command Prompt window and type `pip --version`. You should now see the pip version.

**Additional Notes:**

* If you're using a Python distribution like Anaconda, pip might already be included. Check the documentation for your specific distribution.
* **Using a virtual environment:** It's recommended to use virtual environments to isolate project dependencies. This helps avoid conflicts between different projects. Tools like `venv` (built-in) or `virtualenv` can be used to create virtual environments. Once you activate a virtual environment, you might need to install pip again within that environment.

For more detailed instructions and troubleshooting, refer to the official Python Packaging User Guide: [https://packaging.python.org/tutorials/installing-packages/](https://packaging.python.org/tutorials/installing-packages/)

6. Configure a Database (MySQL):
   Download and install MySQL database. https://dev.mysql.com/downloads/windows/installer/5.7.html
**Downloading MySQL**

1. Visit the official MySQL download page for Windows installers: [https://dev.mysql.com/downloads/mysql/](https://dev.mysql.com/downloads/mysql/)
2. Select the appropriate version based on your system architecture (32-bit or 64-bit). It's recommended to choose the latest stable version (e.g., MySQL 8.0 at the time of writing this).
3. Download the installer (.msi file) by clicking on the corresponding link.

**Installing MySQL**

1. Double-click the downloaded .msi file to launch the installer.
2. Follow the on-screen instructions during the installation process. Here's a general overview of the steps you'll encounter:
    - **Welcome:** Click "Next" to proceed.
    - **License Agreement:** Read the license agreement and select "I accept the license terms and conditions" if you agree. Click "Next".
    - **Choose Setup Type:** Select "Typical" installation for a standard setup or "Custom" if you want more control over the configuration options. Click "Next".
    - **Product Configuration:**
        - **Select Products:** By default, all MySQL products might be selected. You can choose to install only the server components if you don't need additional tools.
        - **Change Installation Directory:** This allows you to specify a custom installation location. The default path is usually `C:\Program Files\MySQL`. Click "Next".
    - **Data Directory:** This is where MySQL stores its data files. You can keep the default path (`C:\Program Data\MySQL`) or choose a custom location. Click "Next".
    - **Security Configuration:** This is a crucial step:
        - **Mode:** It's recommended to choose the "Development Mode" for initial setup and testing purposes. This mode allows easier connection but is less secure for production environments. In production, you'll want to switch to "Strong Configuration Mode" which enforces stricter security measures.
        - **Set Root Password:** Enter a strong password for the root user. This is the most privileged account in MySQL and should be protected carefully. Remember this password as you'll need it to connect to the database server. Click "Next".
    - **Port Configuration:** The default port for MySQL is 3306. You can keep this unless you have a specific reason to change it. Click "Next".
    - **Windows Service Configuration:** This allows you to configure MySQL as a Windows service, enabling it to start automatically when your computer boots up. You can choose a service name and startup type (automatic, manual, etc.). Click "Next".
    - **Ready to Install:** Review the configuration summary and click "Install" to begin the installation process.
    - **Installation Progress:** The installer will copy files and configure the database server.
    - **Completion:** Once the installation is complete, you'll have the option to configure the MySQL Server instance for immediate use. You can check this option if you want to proceed with this step. Click "Finish".

**Post-Installation Steps**

1. If you chose to configure the server instance during installation, the MySQL command line client might launch automatically. You can connect to the server using the root user and the password you set during installation.
2. If you didn't configure the server instance, you'll need to start the service manually. You can do this by searching for "Services" in the Windows search bar, finding the "MySQL80" service (or the service name you chose during installation), right-clicking on it, and selecting "Start".

**Additional Resources**

- MySQL Documentation: [https://dev.mysql.com/doc/](https://dev.mysql.com/doc/)
- Securing a MySQL Server Installation: [https://dev.mysql.com/doc/refman/en/security.html](https://dev.mysql.com/doc/refman/en/security.html)

Remember to choose a strong password for the root user and consider switching to a more secure configuration mode (like "Strong Configuration Mode") for production environments.
7. Set Up Development Environments and Virtualization (Optional):
   Consider using virtualization tools like Docker or virtual machines to isolate project dependencies and ensure consistent environments across different machines.
## Setting Up Development Environments with Virtualization

Virtualization tools like Docker and virtual machines (VMs) are great for isolating project dependencies and creating consistent environments across different machines. Here's a general guide to get you started (specific steps may vary depending on your chosen tool):

### Choosing a Tool: Docker vs. VMs

* **Docker:** More lightweight, focuses on isolating applications with their dependencies. Ideal for smaller, self-contained projects.
* **VMs:** More resource-intensive, creates a complete virtual computer with its own operating system. Better for complex projects requiring specific OS versions or entire software stacks.

**Consider your project needs and resource limitations before choosing.**

### Steps (General)

1. **Pick your tool:** Docker or VM software (e.g., VirtualBox, VMware).
2. **Install the tool:** Download and follow the installation instructions for your chosen tool.
3. **Set up your development environment:**
    * **Docker:**
        * Create a Dockerfile specifying the base image, dependencies, and application setup commands.
        * Build the image using the `docker build` command.
        * Run the container from the image using `docker run`.
    * **VMs:**
        * Create a new virtual machine.
        * Install the desired operating system on the VM.
        * Install the necessary development tools and dependencies within the VM.
4. **Development:**
    * Develop your project within the container/VM.
    * The container/VM isolates your project's environment from your main machine.

**Additional Tips:**

* **Version control:** Use a version control system (e.g., Git) to track changes in your Dockerfile or VM configuration.
* **Sharing environments:** Share your Dockerfile or VM configuration with other developers for easy environment setup.
* **Resources:** There are many resources available online for specific tools and project types. Search for tutorials and documentation related to your chosen tool and development needs.

**Remember, this is a general guide.  For specific instructions, consult the documentation for your chosen tool.**

8. Explore Extensions and Plugins:
   Explore available extensions, plugins, and add-ons for your chosen text editor or IDE to enhance functionality, such as syntax highlighting, linting, code formatting, and version control integration.
**Step 1: Identify your Text Editor/IDE**

First, pinpoint the text editor or IDE you're using. Popular options include Visual Studio Code (VS Code), Sublime Text, Atom, Brackets, and IntelliJ IDEA (for Java development). Each editor has its own extension marketplace.

**Step 2: Access the Extension Marketplace**

Here's a general guideline to find the extension marketplace for some popular editors:

* **VS Code:** Open the Extensions view by clicking on the Extensions icon (usually looks like a box with four squares) on the left sidebar. Alternatively, you can use the shortcut `Ctrl+Shift+X` (Windows/Linux) or `Cmd+Shift+X` (Mac).
* **Sublime Text:** Go to **Preferences** > **Package Control**.
* **Atom:** Open the Settings view by going to **Edit** > **Preferences** (Windows/Linux) or **Atom** > **Preferences** (Mac). Then, search for "Install" and you'll find the "Packages" section.
* **Brackets:** Click on the **Extensions** tab in the Project panel.

**Step 3: Browse and Search for Extensions**

Most marketplaces allow browsing extensions by category or searching for specific functionalities. Here are some functionalities extensions can offer:

* **Syntax Highlighting:** Colors your code based on its structure (keywords, variables, functions) for better readability.
* **Linting:** Identifies potential errors and stylistic inconsistencies in your code.
* **Code Formatting:** Automatically formats your code consistently, improving readability and maintainability.
* **Version Control Integration:** Allows you to connect your editor to version control systems like Git for easier code tracking and collaboration.
* **Code Completion:** Suggests code snippets or function calls as you type, speeding up development.
* **Themes:** Change the look and feel of your editor for a more personalized experience.

**Step 4: Install and Enable Extensions**

Once you find an interesting extension, click the "Install" button in the marketplace. After installation, you might need to restart your editor for the changes to take effect. Some extensions have configuration options you can access through the editor's settings.

**Step 5: Explore and Customize (Optional)**

Many extensions offer additional features or customization options. Play around with the settings to find what works best for you. You can also install and try multiple extensions to create a personalized development environment.

**Additional Tips**

* **Read Reviews:** Before installing an extension, check its user reviews to gauge its reliability and functionality.
* **Start with Essentials:** Begin by installing extensions that address your core needs, like syntax highlighting and linting. You can always add more later.
* **Manage Extensions:** Most marketplaces allow you to disable or uninstall extensions you no longer need.
* **Community Resources:** Look for online communities or forums dedicated to your editor where you can find recommendations for extensions and troubleshooting tips.

By following these steps and exploring the vast world of extensions, you can significantly enhance your coding experience and become a more productive developer!
9. Document Your Setup:
    Create a comprehensive document outlining the steps you've taken to set up your developer environment. Include any configurations, customizations, or troubleshooting steps encountered during the process.
## Setting Up Visual Studio Code (VS Code) on Windows 11

This document outlines the steps for setting up VS Code on a Windows 11 machine, including customizations and any challenges encountered during the process.

**Software:**

* OS: Windows 11
* Code Editor: Visual Studio Code (VS Code)

**Steps:**

1. **Download VS Code:**
    * Visit the official VS Code download page: [download vscode ON Visual Studio code.visualstudio.com]
    * Select the appropriate installer for your system (64-bit or Arm64).

2. **Run the Installer:**
    * Double-click the downloaded installer file (VSCodeSetup-{version}.exe).
    * Click "Yes" or "Run" if prompted for confirmation.

3. **Installation Wizard:**
    * Review the license agreement and click "I accept the agreement" to proceed.
    * Choose a destination folder for VS Code or leave the default location.
    * Optionally, create a desktop shortcut and add VS Code to the PATH environment variable for easier access from the command line.
    * Click "Next" to continue with the installation.

4. **Installation and Completion:**
    * The installer will download and configure VS Code. Wait for the process to finish.
    * Click "Finish" to exit the setup wizard.

**Challenges and Solutions:**

* **Administrator Privileges:** If you encounter permission errors during installation, you might need to run the installer with administrator privileges. Right-click the installer file and select "Run as administrator".

* **Antivirus Software:** Some antivirus software might interfere with the installation. Try temporarily disabling your antivirus and running the installer again. Remember to re-enable it after successful installation.

* **Customizing VS Code:** VS Code offers a wide range of customization options. You can install extensions for specific programming languages, themes to personalize the interface, and configure settings for code formatting, debugging, and more. Explore the VS Code Marketplace ([VS Code Marketplace extension](https://code.visualstudio.com/docs/editor/extension-marketplace)) to discover extensions that suit your development needs.

**Additional Notes:**

* This guide covers the basic installation process. Refer to the official VS Code documentation for more advanced configuration options: [VS Code documentation ON code.visualstudio.com]

* Consider exploring online tutorials and communities for further guidance on setting up VS Code for your specific development workflow.


By following these steps and addressing any potential challenges, you should be able to successfully set up VS Code on your Windows 11 machine and start coding efficiently.
#Deliverables:
- Document detailing the setup process with step-by-step instructions and screenshots where necessary.
- A GitHub repository containing a sample project initialized with Git and any necessary configuration files (e.g., .gitignore).
- A reflection on the challenges faced during setup and strategies employed to overcome them.

#Submission:
Submit your document and GitHub repository link through the designated platform or email to the instructor by the specified deadline.

#Evaluation Criteria:**
- Completeness and accuracy of setup documentation.
- Effectiveness of version control implementation.
- Appropriateness of tools selected for the project requirements.
- Clarity of reflection on challenges and solutions encountered.
- Adherence to submission guidelines and deadlines.

Note: Feel free to reach out for clarification or assistance with any aspect of the assignment.
