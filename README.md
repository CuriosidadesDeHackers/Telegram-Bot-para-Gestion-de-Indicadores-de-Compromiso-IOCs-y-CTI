# 🤖 Telegram Bot para Gestión de Indicadores de Compromiso (IOCs) 📝

Este proyecto consiste en un bot de Telegram que permite a los usuarios agregar Indicadores de Compromiso (IOCs) a un archivo AsciiDoc (`peticiones.adoc`) y luego subirlo a un repositorio de GitHub. El bot está diseñado para funcionar en chats privados y grupos específicos, y utiliza variables de entorno para la configuración.

## ✨ Características

- **Agregar IOCs**: Los usuarios pueden enviar IOCs con detalles específicos (hash, archivo, detección, descripción) que se guardan en un archivo AsciiDoc.
- **Integración con GitHub**: Los IOCs se suben automáticamente a un repositorio de GitHub configurado a través de variables de entorno.
- **Validación de Chats**: El bot solo responde en chats privados con el usuario configurado y en grupos específicos.

## 🛠️ Requisitos

- Node.js
- npm (o yarn)
- Un bot de Telegram (obtén el token de tu bot a través de [BotFather](https://t.me/BotFather))
- Un repositorio de GitHub (configura las variables de entorno necesarias)

## 📦 Instalación

1. **Clona el repositorio**:
    ```bash
    git clone https://github.com/tu-usuario/tu-repositorio.git
    cd tu-repositorio
    ```

2. **Instala las dependencias**:
    ```bash
    npm install
    ```

3. **Configura las variables de entorno**:
    Crea un archivo `.env` en la raíz del proyecto y añade las siguientes variables:
    ```env
    MY_BOT_TOKEN=tu_token_de_telegram
    MY_GITHUB_USER=tu_usuario_de_github
    MY_GITHUB_TOKEN=tu_token_de_github
    MY_GITHUB_REPO=tu_repositorio_de_github
    ```

4. **Inicia el servidor**:
    ```bash
    npm start
    ```

## 📝 Uso

1. **Inicia una conversación con el bot** en Telegram.
2. **Envía el comando `/chatp`** para iniciar el proceso de agregar un IOC.
3. **Responde al mensaje del bot** con los detalles del IOC en el formato solicitado:
    ```
    hash,nombre_del_archivo,detección,descripción
    ```

## 📁 Estructura del Proyecto

- `filemanager.js`: Contiene la lógica para manejar el archivo `peticiones.adoc` y las operaciones de Git.
- `index.js`: Contiene la lógica del bot de Telegram y la configuración del servidor.
- `.env`: Archivo de configuración de variables de entorno.

## 📸 Imágenes

### Captura de Pantalla del Bot en Acción

![1728646983019](https://github.com/user-attachments/assets/73fa0b76-a838-4c29-ba4f-8caa299833f2)
![1728646983199](https://github.com/user-attachments/assets/d10c8796-5a52-4c9a-a07d-1d133f36be07)

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor, abre un issue o envía un pull request para cualquier mejora o corrección.

---

¡Gracias por usar este bot! Si tienes alguna pregunta o sugerencia, no dudes en contactarme. 😊



