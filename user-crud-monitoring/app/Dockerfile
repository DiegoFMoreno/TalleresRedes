FROM python:3.9

# directorio de trabajo
WORKDIR /app

# archivos del proyecto al contenedor
COPY . /app

# dependencias necesarias
RUN pip install --no-cache-dir -r requirements.txt

# puerto
EXPOSE 8000

# Ejecutar el servidor FastAPI
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]