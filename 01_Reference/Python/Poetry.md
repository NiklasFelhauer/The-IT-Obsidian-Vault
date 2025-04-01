
## Show

1. **Show Dependencies:**
   ```shell
poetry show --tree
   ```
## New Package

1. **Create a new Poetry project:**
   ```shell
   poetry new <project_name>
   ```

2. **Create a new project in the current directory:**
   ```shell
   poetry new --src .
   ```

3. **Install dependencies specified in `pyproject.toml`:**
   ```shell
   poetry install
   ```

4. **Update dependencies in `pyproject.toml`:**
   ```shell
   poetry update
   ```

## Add/Remove Dependencies

1. **Add a dependency:**
   ```shell
   poetry add <package_name>
   ```

2. **Add a development dependency:**
   ```shell
   poetry add --dev <package_name>
   ```

3. **Remove a dependency:**
   ```shell
   poetry remove <package_name>
   ```

## Environment Management

1. **Check the status of the virtual environment:**
   ```shell
   poetry env info
   ```

2. **Remove the virtual environment:**
   ```shell
   poetry env remove python
   ```

3. **Use a specific Python version for the environment:**
   ```shell
   poetry env use <python_version>
   ```

## Running Commands

1. **Run a script defined in `pyproject.toml`:**
   ```shell
   poetry run <script_name>
   ```

2. **Run Python code within the Poetry environment:**
   ```shell
   poetry run python <script.py>
   ```

3. **Run tests with pytest:**
   ```shell
   poetry run pytest
   ```

## Publishing

1. **Build the package:**
   ```shell
   poetry build
   ```

2. **Publish to PyPI:**
   ```shell
   poetry publish --username <username> --password <password>
   ```

3. **Publish to a custom repository:**
   ```shell
   poetry publish --repository <repository_name>
   ```

## Configuration and Miscellaneous

1. **Show all Poetry configuration:**
   ```shell
   poetry config --list
   ```

2. **Set a configuration value globally:**
   ```shell
   poetry config <key> <value> --global
   ```

3. **View the lock file for dependency resolution:**
   ```shell
   poetry lock
   ```

4. **Get the version of Poetry:**
   ```shell
   poetry --version
   ```

5. **Get help for any command:**
   ```shell
   poetry help <command>
   ```
