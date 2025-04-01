## Sort

1. **Sort all file imports in a directory:**
   ```shell
   poetry run isort .
   ```

2. **Sort imports in a single file:**
   ```shell
   isort <file_name>
   ```

3. **Sort imports and check for any needed changes (dry run):**
   ```shell
   isort --check-only .
   ```

4. **Sort imports with verbose output:**
   ```shell
   isort . --verbose
   ```

## Configuration

1. **Specify a custom configuration file:**
   ```shell
   isort --settings-path <path_to_config_file>
   ```

2. **Ignore specific files or directories:**
   ```shell
   isort --skip <file_or_directory>
   ```

3. **Use default profiles for specific frameworks (e.g., Django):**
   ```shell
   isort --profile django
   ```

## Formatting

1. **Sort and format using Black compatibility:**
   ```shell
   isort . --profile black
   ```

2. **Ensure only imports are sorted without modifying code structure:**
   ```shell
   isort . --force-single-line-imports
   ```

## Linting

1. **Check for incorrectly sorted imports without fixing:**
   ```shell
   isort . --check-only
   ```

2. **Get detailed output for linting errors:**
   ```shell
   isort . --check-only --verbose
   ```

## Miscellaneous

1. **Show version of ISort:**
   ```shell
   isort --version
   ```

2. **Show help for all commands:**
   ```shell
   isort --help
   ```

---

Feel free to copy and save this content into a file named `isort_cheat_sheet.md`.
