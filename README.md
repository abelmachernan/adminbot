# AdminBot

¡Bienvenido al repositorio de **AdminBot**! Este es un bot de WhatsApp multifuncional diseñado para ayudarte a administrar grupos y ofrecer diversas herramientas a tus usuarios.

## Sobre el Proyecto

**AdminBot** es un bot de WhatsApp basado en [Baileys](https://github.com/adiwajshing/Baileys), modificado para incluir varias funcionalidades útiles para la administración de grupos y la interacción con los usuarios.

**Creador Original**: Fernando  
**Modificado Por**: 『MacHernan』

## Características Principales

- **Sistema de Registro**: Permite a los usuarios registrarse para acceder a ciertas funciones.
- **Manejo de Plugins**: Estructura modular que facilita la adición de nuevas funciones a través de plugins.
- **Manejo de Base de Datos**: Utiliza un archivo JSON (`database.json`) para almacenar datos de usuarios y chats.
- **Limpieza Automática**: Elimina archivos temporales y datos de sesión no esenciales periódicamente.
- **Conexión Flexible**: Soporte para conexión mediante código QR o código de emparejamiento de 8 dígitos.
- **Soporte para Sub-bots (JadiBots)**: Permite la conexión de bots adicionales.
- **Roles de Usuario**: Distintos niveles de permisos (Owner, Mods, Premium, Admin, BotAdmin).
- **Anti-Spam y Baneos**: Funciones básicas para controlar el spam y banear usuarios.
- **Configuraciones de Chat**: Opciones configurables por chat (como bienvenida, antilink, etc.).
- **Funcionalidad solo en grupos con el bot como administrador**: El bot solo responderá a comandos en grupos donde tenga permisos de administrador.

## Instalación

Sigue estos pasos para configurar y ejecutar **AdminBot**:

1. **Clonar el Repositorio**:
   ```bash
   git clone https://github.com/abelmachernan/AdminBot.git
   cd AdminBot
Instalar Dependencias:
Asegúrate de tener Node.js instalado. Luego, instala las dependencias del proyecto:

npm install
# o
yarn install
Configuración Inicial:

Copia el archivo config.js (o similar, si existe) o asegúrate de que tu archivo de configuración (settings.js) esté correctamente configurado con tus ajustes (como el número del bot, propietarios, etc.).
La base de datos se inicializará automáticamente al ejecutar el bot por primera vez en ./src/database/database.json.

Conectar el Bot:
Ejecuta el script principal:

# npm start / node .
El bot te pedirá que elijas un método de conexión (QR o código de 8 dígitos) si no existe una sesión previa. Sigue las instrucciones en la consola para vincular tu número de WhatsApp.

Mantener la Sesión Activa:
Una vez conectado, el bot intentará mantener la sesión activa. Si la conexión se pierde, intentará reconectarse automáticamente.

Uso
Una vez que el bot esté conectado, podrás usar sus comandos en chats individuales o grupos.

Prefijo: El prefijo por defecto para los comandos es #, /, ! o ... Puedes verificar o configurar esto en los archivos de configuración.

Lista de Comandos: La lista completa de comandos se maneja a través del sistema de plugins en la carpeta ./plugins. Cada archivo .js en esta carpeta puede contener uno o varios comandos. Puedes explorar estos archivos para ver los comandos disponibles y su uso.

Comandos de Administración: Algunos comandos solo están disponibles para usuarios con roles específicos (administradores de grupo, propietarios del bot, etc.).

Nota: El bot solo funcionará completamente en grupos donde se le haya otorgado el permiso de administrador.

# Estructura del Proyecto

./               # Archivos principales del bot (index.js, settings.js, etc.)
../lib/          # Librerías y funciones auxiliares (simple.js, database.js, etc.)
../plugins/      # Archivos de plugins que contienen los comandos y funcionalidades del bot
../src/database/ # Contiene el archivo de base de datos (database.json)
../sessions/     # Carpeta donde se guarda la información de la sesión de WhatsApp
../tmp/           # Carpeta para archivos temporales
../JadiBots/      # Carpeta para sesiones de sub-bots

Contribuciones
Si deseas contribuir a este proyecto, puedes hacer un fork del repositorio, realizar tus cambios y enviar un Pull Request.

¡Esperamos que disfrutes usando y modificando AdminBot!
# AdminBot
