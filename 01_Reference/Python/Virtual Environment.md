## Creating a Virtual Environment

1. **Using `venv` (Built-in Python Module):**
    
    ```shell
    python -m venv <env_name>
    ```
    
2. **Using `virtualenv` (External Tool):**
    
    ```shell
    virtualenv <env_name>
    ```
    
3. **Specifying a Python Version:**
    
    ```shell
    python3.8 -m venv <env_name>
    ```
    

## Activating a Virtual Environment

1. **Windows (Command Prompt):**
    
    ```shell
    <env_name>\Scripts\activate
    ```
    
2. **Windows (PowerShell):**
    
    ```shell
    .\<env_name>\Scripts\Activate.ps1
    ```
    
3. **macOS/Linux:**
    
    ```shell
    source <env_name>/bin/activate
    ```
    

## Deactivating a Virtual Environment

To deactivate, simply run:

```shell
deactivate
```

## Deleting a Virtual Environment

1. **Delete the Folder:**
    
    ```shell
    rm -rf <env_name>
    ```
    

## Managing Virtual Environments with `poetry`

1. **Check the Status of the Virtual Environment:**
    
    ```shell
    poetry env info
    ```
    
2. **Remove a Virtual Environment:**
    
    ```shell
    poetry env remove python
    ```
    
3. **Use a Specific Python Version:**
    
    ```shell
    poetry env use <python_version>
    ```
    

## Useful Tips

1. **List All Installed Python Versions:**
    
    ```shell
    pyenv versions
    ```
    
2. **Switch Python Version (Using `pyenv`):**
    
    ```shell
    pyenv global <version>
    ```
    
3. **Verify Active Python Version:**
    
    ```shell
    python --version
    ```