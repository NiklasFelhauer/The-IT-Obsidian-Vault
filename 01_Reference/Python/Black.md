## Sort

1. **Format all files in a directory:**
   ```shell
   poetry run black .
   ```

2. **Format a specific file:**
   ```shell
   black <file_name>
   ```

3. **Check if files need formatting (dry run):**
   ```shell
   black --check .
   ```

4. **Format files and show the diff:**
   ```shell
   black --diff .
   ```

## Line Length

1. **Set a custom line length:**
   ```shell
   black . --line-length <number>
   ```

## Exclude Files or Directories

1. **Exclude specific files or directories:**
   ```shell
   black . --exclude <pattern>
   ```

## Configuration

1. **Use a configuration file (pyproject.toml):**
   ```toml
   [tool.black]
   line-length = 88
   skip-string-normalization = true
   ```
   Then, run:
   ```shell
   black .
   ```

## Miscellaneous

1. **Run Black in verbose mode:**
   ```shell
   black . --verbose
   ```

2. **Show Black's version:**
   ```shell
   black --version
   ```

3. **Get help for Black commands:**
   ```shell
   black --help
   ```
