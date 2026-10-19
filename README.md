Project-azure-storage
📌 Descripción:

Proyecto de desarrollo e integración de servicios en la nube utilizando Microsoft Azure, Twilio y Node.js. Incluye la configuración de recursos en Azure, la creación de un contenedor para almacenar archivos y el desarrollo de una aplicación web con Node.js.

🛠️ Tecnologías y herramientas: Microsoft Azure: infraestructura y servicios en la nube. Azure Blob Storage: almacenamiento de archivos. Twilio: integración de servicios de comunicación. Node.js: entorno de ejecución de JavaScript. Visual Studio Code: editor de código. npm: administrador de paquetes de Node.js. Azure PowerShell y Azure CLI: herramientas para administrar recursos de Azure.

☁️ Configuración de Azure:

Crear un grupo de recursos Crear un grupo de recursos desde Azure Portal y asignar su nombre a la variable $rgName en PowerShell.

Crear una cuenta de almacenamiento Ejecutar en Azure PowerShell: New-AzStorageAccount   -ResourceGroupName $rgName -Name "stgapptwpr2023"   -SkuName Standard_RAGRS -Location "Central US" ` -Kind StorageV2

Crear un contenedor Ejecutar con Azure CLI: az storage container create
--account-name "stgapptwpr2023"
--name "mycontainer"

💻 Configuración de Node.js:

Inicializar el proyecto Desde la terminal, entrar a la carpeta de la aplicación y ejecutar:
npm.cmd init -y

Instalar las dependencias npm.cmd install express express-upload into-stream dotenv azure-storage Estas dependencias permiten preparar el servidor web, gestionar variables de entorno y trabajar con operaciones relacionadas con archivos y almacenamiento.

✅ Lista de tareas:

Crear el grupo de recursos en Azure. Configurar los recursos necesarios para la aplicación web. Crear la cuenta de Azure Storage. Crear el contenedor de almacenamiento. Instalar Node.js y Visual Studio Code. Inicializar el proyecto con npm. Instalar las dependencias. Configurar la integración con Azure Blob Storage. Configurar Twilio según los requisitos del proyecto. Probar el funcionamiento de la aplicación.

🔐 Seguridad:

No subir archivos .env con credenciales al repositorio. No publicar claves de Azure, tokens de Twilio ni contraseñas. Mantener el acceso al almacenamiento restringido cuando no sea necesario hacerlo público.

📚 Estado del proyecto:

Proyecto académico en desarrollo para practicar la configuración e integración de servicios cloud y herramientas de desarrollo web.
