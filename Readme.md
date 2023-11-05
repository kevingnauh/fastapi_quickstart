Quickstart notes to setup a FastAPI project.

## Setup
```
pip install fastapi
```
Install uvicorn to work as the server:
```
pip install "uvicorn[standard]"
```

### Run server:
```
uvicorn main:app --reload
```
Where `main` is name of the main python file and `app` is the FastAPI object.

## Templates
### Simple FastAPI template
`main.py`:
```
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
async def root():
    return {"message": "Hello World"}
```

## Additional
### Notes:
Go to `http://127.0.0.1:8000/docs` to see interactive API documentation (SwaggerUI).   
Go to `http://127.0.0.1:8000/redoc` to see interactive API documentation (ReDoc). 



### Links:
https://fastapi.tiangolo.com/