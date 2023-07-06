# Define la imagen base
FROM python:3

# Establece el directorio de trabajo en /app
WORKDIR /app

# Copia el archivo requirements.txt al directorio de trabajo
COPY requirements.txt .

# Instala las dependencias del proyecto
RUN pip install --no-cache-dir -r requirements.txt

# Copia el contenido del directorio actual al directorio de trabajo
COPY . .

# Expone el puerto 8000 para acceder a la aplicación
EXPOSE 8000

# Ejecuta el comando para iniciar el servidor Django
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
