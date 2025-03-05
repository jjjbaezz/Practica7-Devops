# Usamos la imagen oficial de Python
FROM python:3.9

# Establecemos el directorio de trabajo en el contenedor
WORKDIR /app

# Copiamos el archivo de dependencias y las instalamos
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

# Copiamos el código de la aplicación dentro del contenedor
COPY . .

# Especificamos el comando para ejecutar la aplicación
CMD ["flask", "run", "--host=0.0.0.0"]
