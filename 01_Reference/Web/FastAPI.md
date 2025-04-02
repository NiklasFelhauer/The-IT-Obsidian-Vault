index
## Running a FastAPI Application with Uvicorn

### Run the Application

1. **Basic Run Command:**
    
    ```shell
    uvicorn run:app --reload
    ```
    
2. **Specify Host and Port:**
    
    ```shell
    uvicorn run:app --host 0.0.0.0 --port 8000
    ```
    
3. **Enable Debug Mode:**
    
    ```shell
    uvicorn run:app --reload --log-level debug
    ```
    
4. **Run with Workers (Production Ready):**
    
    ```shell
    uvicorn run:app --workers 4 --host 0.0.0.0 --port 8000
    ```
    

### Tips for FastAPI and Uvicorn

1. **Define Your Application in `run.py`:** Ensure your file contains:
    
    ```python
    from fastapi import FastAPI
    
    app = FastAPI()
    
    @app.get("/")
    def read_root():
        return {"message": "Hello World"}
    ```
    
2. **Install FastAPI and Uvicorn:**
    
    ```shell
    pip install fastapi uvicorn
    ```
    
3. **Use Environment Variables for Configuration:** Leverage `.env` files or `os.environ` for settings like host, port, and debug options.