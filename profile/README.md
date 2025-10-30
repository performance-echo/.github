# Welcome Echoenergia Performance Team! :rocket:

This is the official GitHub organization for Echoenergia's Performance team. Here, we centralize the key Python packages and tools developed and used by our team.

We encourage all team members to contribute! If you've written code that could be reused, this is the place for it. Please ensure your code is well-documented to help your colleagues. For great tips on documentation, see these [Python documenting guidelines](https://realpython.com/documenting-python-code/).

Before you start, please check out our central **[Documentation](https://github.com/performance-echo/documentation)** repository for useful information and standards.

---

## :gear: Getting Started: Environment Setup

To use our packages, you first need to set up your local environment correctly.

### Prerequisites

1.  **Python 3.12**: Our standard environment is Python :snake: 3.12. Ensure you have it installed. We recommend using a version manager like `conda` or `pyenv`.
    ```bash
    # Example using conda
    conda install python=3.12
    ```

2.  **GitHub CLI**: The installation command requires you to be authenticated via the GitHub CLI.
    * **Install it**: If you don't have it, run `winget install --id GitHub.cli` on Windows or follow the [official installation guide](https://github.com/cli/cli#installation) for macOS/Linux.
    * **Authenticate**: After installation, run `gh auth login` and follow the prompts.

3.  **uv Package Installer**: We use `uv` for significantly faster package installation than standard `pip`.
    ```bash
    # Install uv using pip
    pip install uv
    ```

### :package: Installing Team Packages

Once the prerequisites are met, you can install all standard team packages with this single command. It securely downloads the package list and installs them using `uv`.

```bash
 curl -sL -H "Authorization: token $(gh auth token)" -H "Accept: application/vnd.github.v3.raw" "https://api.github.com/repos/performance-echo/.github/contents/echo_packages.txt?ref=main" | uv pip install -r -
```
