#Hoja de trabajo 6
Nombre: Oscar José Cojulún Mendoza Carnet: 9490-22-4974

Descripción:
Esta API permite crear, listar, actualizar y eliminar usuarios. Cada usuario tiene:
- dpi
- name
- email
- password
La API valida que no existan usuarios con el mismo DPI

Instrucciones para ejecutar la API localmente: 
1. Clonar el repositorio
2. Instalar dependencias:
npm install
3. Ejecutar el servidor:
npm start
La API estará disponible en: http://localhost:3000

LA URL no la pude subir a render me tiro error

Descripción de los endpoints con ejemplos de solicitudes y respuestas:

### Crear usuario
POST /users
Body JSON:
{
  "dpi": "12345678",
  "name": "Oscar",
  "email": "oscar@mail.com",
  "password": "1234"
}

### Listar usuarios
GET /users

### Actualizar usuario
PUT /users/:dpi
Body JSON:
{
  "name": "Oscar Mendoza",
  "email": "nuevo@mail.com"
}

### Eliminar usuario
DELETE /users/:dpi
