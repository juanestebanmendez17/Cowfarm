from fastapi import FastAPI

app= FastAPI(
    title = "API Cowfarm",
    description ="frontend cowfarm",
    version ="1.0.0"
)

@app.get ("/")
async def root ():
    """endopoint raiz que retorna en saludo"""
    return {"menssage": "¡Hola, bienvenidos a Cowfarm!"}
