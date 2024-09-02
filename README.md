[![CI](https://github.com/Jourdan0803/ids706-w1/actions/workflows/CI.yml/badge.svg)](https://github.com/Jourdan0803/ids706-w1/actions/workflows/CI.yml)
# ids706-w1
## Setting up

### set up with VS Code and .devcontainer

1. **Install Docker**
2. **Install VS Code Remote - Containers Extensions**: Install the **Remote - Containers** extension in VS Code.
3. **Clone the Repository**: Clone this repository to your local machine using the command:
    ```bash
    git clone 
    ```
4. **Open in VS Code**: Open the repository in Visual Studio Code.
5. **Reopen in Container**: When prompted, click on "Reopen in Container". Alternatively, you can press **command+shift+p**, type "Remote-Containers: Reopen Folder in Container"
6. **Docker Image Build**: The first time you open the project in the container, Docker will build the image as specified in the **Dockerfile**. This may take a few minutes.
7. **Ready-to-Use Environment**: After the setup is complete, you will have a fully configured Python development environment isolated from your local system.

### Running Tests

To run tests and ensure your code is working as expected:

1. **Navigate to the Project Directory**: Open a terminal within VS Code (you should already be in the correct directory if you followed the previous steps).
2. **Run Tests**: Execute the following command to run all unit tests:
    ```bash
    make test
    ```
3. **Review Results**: Check the test output to ensure no new issues were introduced by your changes.
### files
- requirements.txt
- MAKEFILE
- github actions:CI.yml
- .devcontainer
