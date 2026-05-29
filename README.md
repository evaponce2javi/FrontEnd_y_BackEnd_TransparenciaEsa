## Qué tener instalado:
1. Docket Desktop (empaqueta el servicio web Express y PostgreSQL). Hay que abrirlo y luego tendrá el icono de una ballena que debe ponerse en verde.
2. Node JS (Descargar librerías de REACT)
3. VS Code

### Verificar instalación:

```
docker --version
node --version
npm --versión
```
---

## Paso a paso

1. Tener una terminal para el FrontEnd y una terminal para BackEnd, para ello apretar el buscador y escribir "PowerShell".
2. Descomprimir el .zip descargado desde el repositorio, y copiar las rutas de acceso de las carpetas del FontEnd y del BackEnd
3. En la terminal 1 (para el backend) escribir ```cd *rutaDeLaCarpeta*```
4. Con Docker Desktop abierto, ejecutar ```docker compose up -d --build```
5. Estructurar las tablas vacías en PostgreSQL: ```docker compose exec api npx prisma migrate deploy```

6. En la terminal 2 (para el FrontEnd) escribir ```cd *rutaDeLaCarpetaDelFrontEnd*```
7. ```npm install```
8. ```npm run dev```
9. Copiar el localhost y pegarlo en nuestro navegador

### ¿Cómo sabemos si funciona la API?
Debemos ingresar al localhost e ingresar a la ruta /regustro, llenar los campos admin@santodomingo.cl clave123, registrar, crear un departamento y volver al inicio. Finalmente ver si tiene escrito "Datos en vivo".

