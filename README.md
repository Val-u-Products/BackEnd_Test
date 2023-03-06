# BackEnd_Test

Se te ha encomendado la tarea de crear un programa Python que consuma los datos de una API RESTful y los almacene en una base de datos SQL. Se espera que el programa se ejecute automáticamente cada 24 horas y que actualice los datos de la base de datos. La API a consumir es: [https://api.example.com/data ](https://pokeapi.co/) y devuelve una lista de diccionarios con la siguiente estructura:

```
[
  {
    "id": 1,
    "name": "Producto 1",
    "description": "Descripción del producto 1",
    "date": "2022-03-02"
  },
  {
    "id": 2,
    "name": "Producto 2",
    "description": "Descripción del producto 2",
    "date": "2022-03-01"
  },
  {
    "id": 3,
    "name": "Producto 3",
    "description": "Descripción del producto 3",
    "date": "2022-02-28"
  }
]
```
La tabla SQL para almacenar los datos se llama 'products' y tiene la siguiente estructura:

```
CREATE TABLE IF NOT EXISTS products (
    id INTEGER PRIMARY KEY,
    name TEXT,
    base_experience: INTEGER
    height: INTEGER
    is_default: BOOLEAN
    order: INTEGER
    weight: INTEGER
);
```

Tu tarea es escribir un programa Python que consuma los datos de la API, los almacene en la base de datos SQL y se ejecute automáticamente cada 24 horas.
Se espera que el programa cumpla con los siguientes requerimientos:
- El programa debe ser ejecutable en cualquier entorno de Python 3.x
- El programa debe hacer uso de las bibliotecas 'requests' y 'sqlite3'
- El programa debe tener un archivo de configuración donde se especifique la ruta de la base de datos y la frecuencia de actualización de los datos en horas.
- El programa debe tener un registro de eventos donde se guarden los errores y el éxito de la ejecución.
- El programa debe manejar los errores adecuadamente y no fallar en caso de no poder consumir los datos o almacenarlos en la base de datos.

## ¡Buena suerte!
