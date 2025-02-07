# Guía de configuraciones para Unity y Oculus Quest 2

## 1. Requisitos de Programas a Instalar

### Unity
- **Unity Hub**: [Descargar desde Unity](https://unity.com/download)
- **Unity 2022.3.42f1** o una versión compatible con OpenXR.
- Desde Unity Hub, instala Unity con los siguientes módulos:
  - **Android Build Support**
  - **OpenJDK, SDK y NDK** (vienen con Android Build Support)

### (Solo para Windows) Instalar el software de Quest y conectar tu dispositivo
> **Nota**: Si utilizas una Mac, omite este paso.

- En la página de configuración de Quest, descarga e instala la aplicación o el software adecuados para tu dispositivo.
- Dentro de la aplicación, sigue las instrucciones para agregar tu casco, ya sea mediante un cable Link o con Air Link.

### Herramientas de Desarrollo para Android
- **ADB (Android Debug Bridge)**: [Descargar Platform Tools](https://developer.android.com/studio/releases/platform-tools)
- Descomprime `platform-tools.zip` en una carpeta (ejemplo: `C:\adb`) y añádela al `PATH` del sistema para facilitar su uso.

---

## 2. Configuración de Dispositivo Quest

Antes de empezar a desarrollar con un Quest, debes completar algunos pasos para asegurarte de que el dispositivo esté configurado adecuadamente.

### 2.1. Poner el dispositivo en modo desarrollador
1. Sigue las instrucciones que aparecen en la [página para desarrolladores de Oculus](https://developer.oculus.com/) para poner tu dispositivo en modo desarrollador.
2. Esto te permitirá hacer pruebas y desarrollar en tu dispositivo.

### 2.2. Permitir la Depuración USB
1. Conecta los Oculus a la PC mediante un cable USB.
2. Ponte el visor y acepta la solicitud de **Depuración USB**.
   - Marca **"Permitir siempre desde esta computadora"** para no tener que repetir este paso.

### 2.3. Comprobar la Conexión con ADB
1. Abre una terminal en la PC y ejecuta:
   ```sh
   adb devices
2. Si el visor aparece como unauthorized, revisa y acepta la solicitud de depuración en el visor.
