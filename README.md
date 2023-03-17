
## HOW TO PUT IT TO WORK

1. GOOGLE_APPLICATION_CREDENTIALS="mlops...json"
2. Activar el .venv: source .venv/bin/activate

### PARA ACTIVAR LA API:
- Dejar corriendo la API: uvicorn api.main:app

### PARA TESTEAR:
- pytest test.py

### PARA DOCKERIZAR LA API:
- DOCKER_BUILDKIT=1 docker build . -t model-api:v1
- docker run -p 8001:8000 model-api:v1. In this case, it could be 8000:8000 but it is already being used. 
