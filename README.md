# Argentina Provinces and Cities

[![GitHub repo](https://img.shields.io/badge/GitHub-ar--ubicaciones-black?logo=github)](https://github.com/joelcolombo/ar-ubicaciones)

This repository contains a complete list of **provinces** and **cities** in Argentina in JSON format, designed for simple integrations where you need to relate each city to its corresponding province.


## Why use this repository
✅ **Simple and free alternativ**e to the Georef API.  
✅ No transfer limits or request throttling.  
✅ Preprocessed data, ready to use in any project.  
✅ Lightweight format, perfect for forms, selectors, and autocompletes.  
✅ No dependencies or authentication required.  


## Available files
[`provincias.json`](./data/provincias.json) — List of provinces with `id` and `nombre` (name).  
[`ciudades.json`](./data/ciudades.json) — List of cities with `id`, `nombre` (name), and `provincia_id` to match them with provinces.  

🔗 **Direct download:** [Provinces](https://raw.githubusercontent.com/joelcolombo/ar-ubicaciones/main/data/provincias.json) — [Cities](https://raw.githubusercontent.com/joelcolombo/ar-ubicaciones/main/data/ciudades.json)  


## Demo
```javascript
// English
const provincesUrl = "https://raw.githubusercontent.com/joelcolombo/ar-ubicaciones/main/data/provincias.json";
const citiesUrl = "https://raw.githubusercontent.com/joelcolombo/ar-ubicaciones/main/data/ciudades.json";

async function loadData() {
  const provinces = await fetch(provincesUrl).then(r => r.json());
  const cities = await fetch(citiesUrl).then(r => r.json());
  console.log(provinces); // List of provinces
  console.log(cities);    // List of cities
}
```


## Data format
### Example provincias.json:
[
  { "id": "1", "nombre": "Buenos Aires" },
  { "id": "2", "nombre": "Catamarca" }
]

### Example ciudades.json:
[
  { "id": "1", "nombre": "La Plata", "provincia_id": "1" },
  { "id": "2", "nombre": "El Desmonte", "provincia_id": "2" }
]


## License
This dataset is free to use. You can use it in personal or commercial projects without restrictions.


---


# Provincias y Ciudades de Argentina

[![GitHub repo](https://img.shields.io/badge/GitHub-ar--ubicaciones-black?logo=github)](https://github.com/joelcolombo/ar-ubicaciones)

Este repositorio contiene un listado completo de **provincias** y **ciudades** de Argentina en formato JSON, pensado para integraciones simples donde sea necesario relacionar cada ciudad con su provincia correspondiente.


## Por qué usar este repositorio
✅ **Alternativa simple y gratuita** al API de Georef.
✅ Sin límites de transferencia ni bloqueos por exceso de consultas.
✅ Datos preprocesados y listos para usar en cualquier proyecto.
✅ Formato liviano, ideal para formularios, selectores y autocompletados.
✅ No requiere dependencias ni autenticación.


## Archivos disponibles
[`provincias.json`](./data/provincias.json) — Listado de provincias con `id` y `nombre`.
[`ciudades.json`](./data/ciudades.json) — Listado de ciudades con `id`, `nombre` y `provincia_id` para relacionarlas con provincias.

🔗 **Descarga directa:** [Provincias](https://raw.githubusercontent.com/joelcolombo/ar-ubicaciones/main/data/provincias.json) — [Ciudades](https://raw.githubusercontent.com/joelcolombo/ar-ubicaciones/main/data/ciudades.json)  


## Ejemplo de uso
```javascript
// Español
const provinciasUrl = "https://raw.githubusercontent.com/joelcolombo/ar-ubicaciones/main/data/provincias.json";
const ciudadesUrl = "https://raw.githubusercontent.com/joelcolombo/ar-ubicaciones/main/data/ciudades.json";

async function cargarDatos() {
  const provincias = await fetch(provinciasUrl).then(r => r.json());
  const ciudades = await fetch(ciudadesUrl).then(r => r.json());
  console.log(provincias); // Lista de provincias
  console.log(ciudades);   // Lista de ciudades
}
```


## Formato de datos
### Ejemplo provincias.json:
[
  { "id": "1", "nombre": "Buenos Aires" },
  { "id": "2", "nombre": "Catamarca" }
]

### Ejemplo ciudades.json:
[
  { "id": "1", "nombre": "La Plata", "provincia_id": "1" },
  { "id": "2", "nombre": "El Desmonte", "provincia_id": "2" }
]


## Licencia
Este dataset es de uso libre. Podés usarlo en proyectos personales o comerciales sin restricción.
