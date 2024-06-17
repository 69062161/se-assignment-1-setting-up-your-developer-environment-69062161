[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/vbnbTt5m)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15287002&assignment_repo_type=AssignmentRepo)
# Dev_Setup
Setup Development Environment

#Assignment: Setting Up Your Developer Environment

#Objective:
This assignment aims to familiarize you with the tools and configurations necessary to set up an efficient developer environment for software engineering projects. Completing this assignment will give you the skills required to set up a robust and productive workspace conducive to coding, debugging, version control, and collaboration.

#Tasks:

1. Select Your Operating System (OS):
   Choose an operating system that best suits your preferences and project requirements. Download and Install Windows 11. https://www.microsoft.com/software-download/windows11
   I have successfully installed windows 11.

2. Install a Text Editor or Integrated Development Environment (IDE):
   Select and install a text editor or IDE suitable for your programming languages and workflow. Download and Install Visual Studio Code. https://code.visualstudio.com/Download
   I have successfully installed visual studio.

3. Set Up Version Control System:
   Install Git and configure it on your local machine. Create a GitHub account for hosting your repositories. Initialize a Git repository for your project and make your first commit. https://github.com
   I have successfully installed GIt and configured it.

4. Install Necessary Programming Languages and Runtimes:
  Instal Python from http://wwww.python.org programming language required for your project and install their respective compilers, interpreters, or runtimes. Ensure you have the necessary tools to build and execute your code.
  I have successfully installed python.

5. Install Package Managers:I have successfully installed windows 11.
   If applicable, install package managers like pip (Python).
   I have successfully installed.


6. Configure a Database (MySQL):
   Download and install MySQL database. https://dev.mysql.com/downloads/windows/installer/5.7.html
   I have successfully installed Mysql.

7. Set Up Development Environments and Virtualization (Optional):
   Consider using virtualization tools like Docker or virtual machines to isolate project dependencies and ensure consistent environments across different machines.

Setting up development environments using virtualization tools like Docker or virtual machines can greatly enhance productivity and ensure consistency across different machines. Here’s a guide on how to set up such environments:

### Docker

**1. Install Docker:**
   - Docker provides containers that encapsulate software environments. Install Docker from [Docker's official website](https://www.docker.com/get-started).

**2. Create a Dockerfile:**
   - Dockerfile defines the environment setup. Here's a basic example for a Node.js application:
     ```dockerfile
     # Use an official Node.js runtime as a parent image
     FROM node:14

     # Set the working directory in the container
     WORKDIR /app

     # Copy package.json and package-lock.json to the working directory
     COPY package*.json ./

     # Install dependencies
     RUN npm install

     # Copy the rest of the application code to the working directory
     COPY . .

     # Expose the port the app runs on
     EXPOSE 3000

     # Command to run the application
     CMD ["node", "app.js"]
     ```

**3. Build the Docker Image:**
   - Navigate to the directory containing the Dockerfile and run:
     ```
     docker build -t my-node-app .
     ```

**4. Run the Docker Container:**
   - Start a container from the image:
     ```
     docker run -p 3000:3000 my-node-app
     ```

   - Now, your Node.js application is running in a Docker container, isolated from your host environment.

### Virtual Machines (using VirtualBox as an example)

**1. Install VirtualBox:**
   - VirtualBox is a free and open-source virtualization software. Download and install it from [VirtualBox's official website](https://www.virtualbox.org/).

**2. Create a Virtual Machine:**
   - Open VirtualBox and click on "New" to create a new virtual machine.
   - Follow the wizard to set up the VM, specifying the operating system and allocating resources like RAM and disk space.

**3. Install Guest OS:**
   - Install the operating system within the VM using an ISO image or installation media.

**4. Set Up Development Environment:**
   - Install necessary software and dependencies inside the VM, just as you would on a physical machine.

**5. Snapshot (Optional):**
   - VirtualBox allows you to take snapshots of VM states, which can be useful for reverting to a clean state or for testing purposes.

### Benefits of Using Docker or Virtual Machines:

- **Isolation:** Ensures that dependencies and configurations are consistent across different machines.
- **Portability:** Easily shareable and transferable environments.
- **Scalability:** Quickly replicate environments for testing or development purposes.
- **Consistency:** Eliminates "it works on my machine" issues by standardizing environments.

8. Explore Extensions and Plugins:
   Explore available extensions, plugins, and add-ons for your chosen text editor or IDE to enhance functionality, such as syntax highlighting, linting, code formatting, and version control integration.

Exploring extensions, plugins, and add-ons for text editors and IDEs can significantly enhance productivity and functionality. Here are some popular tools across different editors:

### Visual Studio Code (VS Code):
1. **ESLint**: Linting tool for JavaScript and TypeScript.
2. **Prettier**: Code formatter that supports various languages.
3. **GitLens**: Git integration with powerful features like blame annotations and repository history viewing.
4. **Live Server**: Launches a local development server with live reload capability.
5. **Bracket Pair Colorizer**: Colorizes matching brackets to make code blocks more readable.
6. **Path Intellisense**: Autocompletes filenames in import statements.
7. **Docker**: Adds syntax highlighting, commands, and more for Dockerfiles and docker-compose.yml files.

### Sublime Text:
1. **Package Control**: Package manager for installing plugins like Emmet, SublimeLinter, etc.
2. **Emmet**: Expedites writing HTML and CSS with shorthand syntax.
3. **SublimeLinter**: Provides linting for various languages.
4. **Git**: Provides Git integration for version control.
5. **AdvancedNewFile**: Simplifies creating and navigating files.

### Atom:
1. **Teletype**: Real-time collaboration in Atom.
2. **Atom Beautify**: Formats code in various languages.
3. **Minimap**: Provides a preview of the full source code.
4. **File Icons**: Adds file-specific icons in the file tree for better visualization.
5. **PlatformIO IDE Terminal**: Integrated terminal for managing projects.

### JetBrains IDEs (e.g., IntelliJ IDEA, PyCharm, PhpStorm):
1. **Code Inspections**: Built-in code quality analysis and suggestions.
2. **Version Control Integration**: Git, SVN, Mercurial integration.
3. **Database Tools**: Database management and integration.
4. **Plugin Repository**: Access to a wide range of plugins specific to the IDE's ecosystem.
5. **Language Support**: Extensive support for various programming languages and frameworks.

### Notepad++:
1. **NppExec**: Plugin for running scripts and commands within Notepad++.
2. **Compare**: Allows comparison of two files.
3. **Explorer**: Adds a file explorer panel for navigation.
4. **AutoSave**: Automatically saves files periodically.

### Eclipse:
1. **EGit**: Git integration for version control.
2. **FindBugs**: Detects potential bugs in Java code.
3. **JUnit**: Unit testing framework integration.
4. **Maven Integration**: Build automation tool integration.

### Emacs:
1. **Magit**: Git integration within Emacs.
2. **Flycheck**: On-the-fly syntax checking.
3. **Yasnippet**: Template system for inserting frequently used text snippets.

9. Document Your Setup:
    Create a comprehensive document outlining the steps you've taken to set up your developer environment. Include any configurations, customizations, or troubleshooting steps encountered during the process. 
    Sure, here's a summary based on the information provided:

**Summary of the Request:**

The task is to create a detailed document that documents the setup of a developer environment. This document should include steps taken to configure the environment, any customizations made, and how any encountered issues were resolved. Additionally, it should cover the optional use of virtualization tools like Docker or virtual machines to ensure consistent environments and isolate project dependencies.

**Key Points to Include:**

1. **Environment Setup:**
   - Document the initial setup of the development environment, including operating system installation, IDE setup (e.g., Visual Studio Code, IntelliJ IDEA), and installation of necessary development tools (e.g., Git, Node.js, Python).

2. **Configuration and Customization:**
   - Detail any specific configurations or customizations made to tailor the environment to project requirements. This may include setting environment variables, configuring network settings, or integrating with specific APIs or services.

3. **Troubleshooting Steps:**
   - Describe any issues encountered during the setup process and how they were resolved. This could involve troubleshooting IDE configurations, resolving compatibility issues between software versions, or addressing installation errors.

4. **Optional Use of Virtualization Tools:**
   - Explain the rationale for using virtualization tools such as Docker or virtual machines to manage project dependencies and ensure consistent environments across different machines. Outline the steps taken to set up Docker containers or virtual machines if applicable.

5. **Documentation Best Practices:**
   - Emphasize the importance of clear documentation practices throughout the process to ensure that setup steps are reproducible and understandable by team members or future developers.

By following these guidelines, the document will provide a comprehensive guide to setting up a developer environment, covering both basic setup steps and optional advanced practices like virtualization for enhanced environment consistency and isolation.


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
