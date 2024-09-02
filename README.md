[![CI](https://github.com/Jourdan0803/ids706-w1/actions/workflows/CI.yml/badge.svg)](https://github.com/Jourdan0803/ids706-w1/actions/workflows/CI.yml)

---

## Setup with VS Code and .devcontainer

Follow these steps to prepare and use your development environment:

### Prerequisites

- **Docker**: Ensure Docker is installed and running on your machine. [Download Docker](https://docs.docker.com/get-docker/).
- **Visual Studio Code**: Install VS Code if you haven't already. [Download VS Code](https://code.visualstudio.com/Download).
- **Remote - Containers Extension**: Install the **Remote - Containers** extension in VS Code by searching for it in the Extensions view (`Ctrl+Shift+X`).

### Getting Started

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   ```
   Replace `<repository-url>` with the actual URL of the repository.

2. **Open in VS Code**:
   Open the cloned repository folder in Visual Studio Code.

3. **Reopen in Container**:
   When prompted in VS Code, click on "Reopen in Container" to start working inside a Docker container. Alternatively, use the Command Palette (`Cmd+Shift+P` on macOS or `Ctrl+Shift+P` on Windows/Linux) and select **Remote-Containers: Reopen Folder in Container**.

4. **Build Docker Image**:
   On the first launch in a container, Docker will build the development environment as specified in the `.devcontainer/Dockerfile`. This process may take a few minutes depending on your internet connection and computer speed.

5. **Development Environment Ready**:
   Once the container setup is complete, you will have a fully configured Python development environment ready for use.

### Running Tests

To ensure your code modifications function correctly:

1. **Open Terminal in VS Code**:
   Use the integrated terminal in VS Code (`Ctrl+``), ensuring you are at the project root directory.

2. **Execute Tests**:
   Run the tests using the Makefile command:
   ```bash
   make test
   ```

3. **Review Test Results**:
   Examine the output in the terminal to verify that all tests pass without errors.

### Project Structure

Here is an overview of important files and directories in the repository:

- `.devcontainer/`: Contains Docker configuration files for setting up the development environment.
- `.github/workflows/`: Includes CI/CD pipeline configurations using GitHub Actions.
- `Makefile`: Defines scripts for common project tasks such as testing.
- `README.md`: Provides project documentation.
- `main.py`: Main Python application file.
- `requirements.txt`: Lists all Python dependencies.
- `test_main.py`: Contains unit tests for the application.

---

This revised README provides clear, step-by-step instructions and organizes information in a structured manner, making it easier for users to set up their environment and understand the project layout. Adding direct links to download necessary software and a brief description of each major file and directory enhances the documentation's utility and user-friendliness.
