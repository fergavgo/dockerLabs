# que imagen vamos a usar?
FROM node

# indicar el directorio de trabajo
WORKDIR /app

# comandos a correr dentro del contenedor
# CUANDO SE ESTA CREANDO LA IMAGEN
COPY package.json /app

RUN npm install

EXPOSE 1080

# que archivos vamos a copiar? 
# todos los de este directorio a la carpeta /app
# se puede indicar "." porque ya "estamos" en el WORKDIR 
# que se indico antes
COPY . /app

# comandos a correr dentro del contenedor
# CUANDO YA LA IMAGEN HA SIDO CREADA
# esa es la diferencia entre RUN y CMD
CMD ["node", "server.js"]