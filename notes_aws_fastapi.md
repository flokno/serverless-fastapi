AWS and FastAPI
===

https://www.deadbear.io/simple-serverless-fastapi-with-aws-lambda/

activate conda env

```bash
conda activate ./conda_env
```



main file:

```python
from fastapi import FastAPI

app = FastAPI()


@app.get("/")
async def root():
  return {"message": "Hello World"}
```

run fastapi

```bash
uvicorn main:app --reload
```

open browser

```
http://localhost:8000/docs
```

