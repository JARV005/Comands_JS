# Comands_JS

✅ 1. Actualizar tu sistema
Primero, asegúrate de que tu sistema esté actualizado.

bash
Copiar
Editar
sudo apt update && sudo apt upgrade -y   # Para Debian, Ubuntu
✅ 2. Instalar cURL y herramientas necesarias
bash
Copiar
Editar
sudo apt install curl git -y
✅ 3. Instalar Node.js (versión estable LTS)
Usa nvm (Node Version Manager), la forma más segura y flexible.

bash
Copiar
Editar
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
Después de eso, reinicia la terminal o ejecuta:

bash
Copiar
Editar
source ~/.bashrc  # o ~/.zshrc si usas Zsh
Ahora instala Node.js:

bash
Copiar
Editar
nvm install --lts
nvm use --lts
nvm alias default lts/*
Verifica:

bash
Copiar
Editar
node -v
npm -v
✅ 4. Instalar un servidor web local (opcional)
Si necesitas servir archivos HTML/JS en local, puedes instalar live-server:

bash
Copiar
Editar
npm install -g live-server
Y luego simplemente navega a tu proyecto y corre:

bash
Copiar
Editar
live-server
✅ 5. Instalar JSON Server (para pruebas de API)
Si tu prueba incluye consumir APIs, simular un backend o hacer un CRUD, instala json-server:

bash
Copiar
Editar
npm install -g json-server
Luego puedes crear un archivo db.json y levantar el servidor con:

bash
Copiar
Editar
json-server --watch db.json --port 3000
✅ 6. Instalar un editor si no tienes (opcional)
Si aún no tienes Visual Studio Code:

bash
Copiar
Editar
sudo snap install code --classic  # Para distros con Snap
✅ 7. Otros útiles (opcional)
bash
Copiar
Editar
npm install -g nodemon      # Para reiniciar auto al trabajar con Node
npm install -g http-server  # Otra opción para servir archivos
📁 Ejemplo de estructura mínima para pruebas JS
bash
Copiar
Editar
mkdir prueba-js
cd prueba-js
touch index.html script.js style.css
code .
