# Tema 3: El poder de la linea de comandos:

### 📍Comparctar y comprimir comando tar

- **El comando tar sirve para compactar varios ficheros y directorios en un sólo archivo**

    - Mediante opciones podemos comprimir el fichero resultando
    utilizando distintos métodos de compresión
    - Sintaxis: tar [opciones] destino.tar datos
    - Uso básico. Compactar: tar -cf fichero.tar /etc/ /var/
    Extraer: tar -xf fichero.tar
    - Comprimir con gzip: **tar -czf fichero.tar.gz /etc/ /var/**
    - Extraer: **tar -xzf fichero.tar.gz**

- **Opciones para copias de seguridad**

    - Totales: se copian todos los datos
    - Diferenciales: se copian sólo los que se hayan modificado desde una fecha indicada. Se utiliza la opción -N seguido de la fecha
    - Incrementales: se copian sólo los ficheros que se han modificado desde la última copia. Se utiliza la opción -g seguido de la ruta del fichero de registro.

- **Opciones más importantes**:

    - c : compacta
    - x : expande (extrae)
    - f : escribe o lee de un fichero
    - z : comprime o descomprime con gzip
    - j : comprime o descomprime con bzip2
    - P : utiliza rutas absolutas (por defecto serán relativas)
    - p : preserva los permisos de los ficheros originales
    - r : añade elementos a un fichero compactado
    - t : muestra la información que contiene un fichero tar

### Practica con tar