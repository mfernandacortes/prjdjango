# Introducción a MongoDB

## Instalación de MongoDB

1. Ingresar al sitio oficial de MongoDB:
   
   https://www.mongodb.com

2. Ir a la sección **Download**.

3. Descargar la versión **Community Server**.

4. Ejecutar el instalador `.msi` y completar la instalación.

---

## Crear carpeta de almacenamiento

En el disco donde se instaló MongoDB:

1. Crear una carpeta llamada:

```text
data
```

2. Dentro de `data`, crear otra carpeta:

```text
db
```

Esta carpeta almacenará la información de las bases de datos.

---

## Ubicación de los ejecutables

Buscar la carpeta:

```text
MongoDB/Server/4.2/bin
```

Allí se encuentran los ejecutables:

- `mongo`
- `mongod`

---

## Iniciar MongoDB

### Abrir el servidor

Ejecutar:

```text
mongod
```

Verificar que aparezca el mensaje:

```text
waiting for connections on port 27017
```

Esto indica que el servidor está funcionando correctamente.

---

### Abrir el cliente

Ejecutar:

```text
mongo
```

---

# Ejercitación

## Consigna

En una mueblería se solicita registrar la siguiente información:

### Clientes
- DNI
- Apellido y Nombre
- Teléfono

### Productos
- Detalle
- Precio
- Cantidad

---

## Actividades

1. Crear una base de datos.

2. Crear las colecciones:
   - `clientes`
   - `productos`

3. Agregar:
   - 5 documentos en `productos`
   - 3 documentos en `clientes`

4. Mostrar los datos ingresados en forma ordenada.

5. Eliminar un cliente.

6. Modificar la cantidad de uno de los productos.