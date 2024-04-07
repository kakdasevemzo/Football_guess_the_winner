# AIBG

## GitHub Cooperation

### Initial Setup
To contribute to the AIBG project, start with the following setup steps:

1. **Clone the Repository**: Obtain a local copy of the repository.
    ```bash
    git clone https://github.com/kakdasevemzo/AIBG
    ```
2. **Create a New Branch**: Create your feature or bugfix branch.
    ```bash
    git checkout -b <branch-name>  # This can be your name or a brief description of the change
    ```
3. **Set Tracking Branch**: Ensure your branch tracks the `main` branch. This keeps you updated with the latest changes in `main`.
    ```bash
    git branch --set-upstream-to=origin/main
    ```

### Workflow
Follow this workflow for contributing changes:

1. **Pull Latest Changes**: Always start by pulling the latest changes from the `main` branch to avoid conflicts.
    ```bash
    git pull --rebase
    ```
2. **Make Changes**: Implement your feature, enhancement, or bugfix in your branch.
3. **Push Changes to Your Branch**: After committing your changes, push them to your branch on GitHub.
    ```bash
    git push origin <branch-name>
    ```
4. **Create a Pull Request**: On GitHub, open a pull request (PR) for your branch against the `main` branch.
5. **Merge the Pull Request**: If the automated pipelines pass merge the PR into `main`.

## Setup Environment and Install Dependencies

Before starting development, set up your environment and install dependencies:

```bash
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### Adding New Dependencies
If you add new dependencies to the project, update the `requirements.txt`.


### Run before commit
To maintain high code quality, run these commands before committing your changes:
```bash
    isort . # Sort imports
    black . # Format code
    mypy . # Type check
    pytest # Run tests
```
Adhering to these practices ensures that your contributions are consistent which makes cooperation easier.

## Conclusion

This markdown is designed to offer a comprehensive guide for setting up the development environment, contributing to the project, and ensuring code quality, all in a clear and structured format suitable for your README file.
