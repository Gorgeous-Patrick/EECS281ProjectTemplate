# EECS 281 Devcontainer Template

Welcome to the EECS 281 Devcontainer Template! This repository provides a ready-to-use development environment for EECS 281 students with essential tools pre-installed, such as `valgrind`, `perf`, `clang`, `gcc`, `g++`, and `clang++`. 

Please note: This repository is **experimental** and is **not officially supported** by the course staff. You can use it if you encounter issues setting up your local development environment.

---

## Features
- **Pre-installed Tools:** 
  - `valgrind`: For memory leak detection.
  - `perf`: For performance profiling.
  - `clang`/`clang++`: Powerful C++ compilers.
  - `gcc`/`g++`: The GNU C++ Compilers.
- A consistent and portable development environment using Docker.

---

## Prerequisites
To use this devcontainer, ensure you have the following installed on your computer:

1. **Docker**
   - Download and install Docker Desktop:
     - [Windows/Mac](https://www.docker.com/products/docker-desktop/)
     - [Linux](https://docs.docker.com/engine/install/)

2. **VS Code (Visual Studio Code)**
   - Download and install VS Code: [VS Code Download](https://code.visualstudio.com/)

3. **Remote - Containers Extension for VS Code**
   - Install the extension: [Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

---

## How to Use
Follow the step-by-step guide below to get started:

### Step 1: Generate Your Own Repository
This repository is a GitHub template, allowing you to create your own copy of it easily.

1. Navigate to the repository: [EECS 281 Project Template](https://github.com/Gorgeous-Patrick/EECS281ProjectTemplate).
2. Click the green **"Use this template"** button.
3. Follow the prompts to create your own repository based on this template.

### Step 2: Clone Your New Repository
After generating your own repository, clone it to your local machine:
```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### Step 3: Open the Repository in VS Code
1. Launch VS Code.
2. Open the folder you just cloned:
   - Go to `File > Open Folder` and select your project directory.

### Step 4: Open in the Devcontainer
1. When you open the repository in VS Code, it will prompt you to reopen the folder in the container.
   - If prompted, click **"Reopen in Container"**.
2. If you don’t see the prompt, press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac) to open the Command Palette.
   - Type **"Remote-Containers: Reopen in Container"** and select it.

### Step 5: Wait for the Container to Build
The container setup may take a few minutes during the first run as it downloads and installs dependencies. Once it completes, you’ll be inside the devcontainer.

### Step 6: Verify the Setup
To ensure everything is working:

1. Open a terminal in VS Code (`Ctrl+`` or View > Terminal`).
2. Run the following commands:
   ```bash
   gcc --version  # Check GCC installation
   g++ --version  # Check G++ installation
   clang --version  # Check Clang installation
   clang++ --version  # Check Clang++ installation
   valgrind --version  # Check Valgrind installation
   perf --version  # Check Perf installation
   ```
3. Each command should output the respective version information, confirming the tools are installed.

---

## Using GitHub Codespaces
If you prefer to work online, you can use GitHub Codespaces to create and develop your projects directly in the browser:

### Step 1: Enable Codespaces
1. Navigate to your repository on GitHub.
2. Click the **"Code"** button, then select the **"Codespaces"** tab.

### Step 2: Start a Codespace
1. Under the Codespaces tab, click **"Create codespace on main"**.
2. Wait for the environment to set up (this may take a few minutes).

### Step 3: Develop in the Browser
Once the Codespace is ready, you’ll be in a VS Code-like environment in your browser:
1. Open a terminal and verify the setup as shown in Step 6 above.
2. Begin coding and testing your projects directly online!

### Notes on Codespaces
- Files will be saved automatically, and changes are synced to your repository.
- Ensure you push your commits regularly to avoid losing progress.

---

## Troubleshooting

### Common Issues:
1. **Docker not running**
   - Ensure Docker Desktop is running on your computer before starting VS Code.

2. **Reopen in Container option not available**
   - Make sure you have the Remote - Containers extension installed.
   - Restart VS Code if necessary.

3. **Build Errors**
   - Ensure you have a stable internet connection, as Docker needs to download images during the build process.

If you encounter other issues, feel free to reach out for assistance.

---

## Notes
- This devcontainer setup is **optional** and **experimental**. It hopefully helps you when you have problems setting up your local environment. Feel free to give it a try.
- Always ensure your work is backed up, as this environment does not automatically sync files outside the container unless you explicitly save them.

Happy Coding!