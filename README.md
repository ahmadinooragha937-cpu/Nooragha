from fastapi import FastAPI

app = FastAPI()

@app.get("/")

def home():

    return {"message": "AI App Works"}

@app.get("/chat")

def chat(message: str):

    return {"response": "AI جواب: " + message}