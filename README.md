# KitsuDroid Mobile 🦊

![Version](https://img.shields.io/badge/version-v1.0-orange?style=for-the-badge)
![Platform](https://img.shields.io/badge/platform-Android%20(ARMv7)-green?style=for-the-badge)
![License](https://img.shields.io/badge/license-Proprietary-red?style=for-the-badge)

**KitsuDroid Mobile** es un IDE ligero y portátil para Android que te permite crear, editar y compilar aplicaciones Java y C/C++ directamente desde tu teléfono. Utiliza un entorno Debian (mediante PRoot) y el SDK de Android para ofrecer una experiencia de desarrollo real, sin necesidad de una PC.

> ⚠️ **Nota:** Este repositorio solo contiene los archivos de distribución (rootfs y APK). El código fuente es privado.

---

## 📥 Descargas

Todos los archivos necesarios están disponibles en la sección de **[Releases](https://github.com/DayFoxAnims/KitsuDroid-Mobile/releases)**. Debes descargar los siguientes archivos:

| Archivo | Descripción | ¿Obligatorio? |
| :--- | :--- | :--- |
| `KitsuDroid-armeabi-v7a.apk` | La aplicación KitsuDroid Mobile. | ✅ Sí |
| `debian-kitsudroid.tar.xz` | Rootfs de Debian 13 (Trixie) ARMHF. Entorno donde se ejecutan las herramientas de compilación. | ✅ Sí |
| `android-ndk-r29-arm-linux-gnueabihf.tar.xz` | Android NDK custom para compilar código nativo (C/C++). | ⚠️ Opcional (Requerido solo si compilas apps con C/C++) |

### 🔗 Enlaces directos (v1.0)

- **APK:** [KitsuDroid-armeabi-v7a.apk](https://github.com/DayFoxAnims/KitsuDroid-Mobile/releases/download/v1.0/KitsuDroid-armeabi-v7a.apk)
- **Rootfs Debian:** [debian-kitsudroid.tar.xz](https://github.com/DayFoxAnims/KitsuDroid-Mobile/releases/download/v1.0/debian-kitsudroid.tar.xz)
- **NDK (Opcional):** [android-ndk-r29-arm-linux-gnueabihf.tar.xz](https://github.com/HomuHomu833/android-ndk-custom/releases/download/r29/android-ndk-r29-arm-linux-gnueabihf.tar.xz)

---

## 🚀 Instalación y Primer Uso

1. **Instala el APK:**
   - Descarga `KitsuDroid-armeabi-v7a.apk` y ábrelo en tu dispositivo para instalarlo. (Es posible que debas activar "Instalar apps de fuentes desconocidas" en los ajustes de Android).

2. **Concede permisos:**
   - Abre la app y sigue las instrucciones de la pantalla de bienvenida. Necesitarás conceder el permiso de **"Acceso a todos los archivos"** para que KitsuDroid pueda leer y escribir proyectos en el almacenamiento.

3. **Instala el Rootfs (Obligatorio):**
   - En la pantalla de bienvenida, selecciona el archivo `debian-kitsudroid.tar.xz` que descargaste.
   - La app extraerá el entorno Debian. Este proceso puede tardar varios minutos.

4. **Configura el SDK (Obligatorio para compilar):**
   - Ve a **Ajustes del IDE → SDK**.
   - Selecciona un archivo `android.jar` (puedes obtenerlo del SDK de Android o de tu instalación de Termux). La app lo copiará automáticamente al entorno Debian.

5. **Configura el NDK (Opcional):**
   - Si vas a compilar proyectos con código nativo (C/C++), ve a **Ajustes del IDE → NDK**.
   - Selecciona el archivo `android-ndk-r29-arm-linux-gnueabihf.tar.xz`. La app lo extraerá y configurará las variables de entorno automáticamente.

6. **¡A programar!**
   - Crea un nuevo proyecto desde la pantalla principal o abre uno existente. Usa el editor para escribir tu código y pulsa el botón de **Compilar** (▶️) para generar el APK.

---

## 🛠️ Características Principales

- **Editor de código** con resaltado de sintaxis para Java, XML, C y C++.
- **Explorador de archivos** con iconos por tipo de archivo y estructura de árbol.
- **Terminal integrada** con soporte para PRoot (entorno Debian real).
- **Compilación nativa** de apps Java y C/C++ (con NDK).
- **Asistente de IA** integrado (soporta DeepSeek, OpenAI, Claude, Gemini y URLs personalizadas).
- **Interfaz oscura** optimizada para programar.

---

## ❓ Preguntas Frecuentes

**¿Por qué el APK es tan grande?**
El APK base es ligero (~8 MB). El tamaño total se debe al rootfs de Debian (210 MB) y al NDK (194 MB), que se descargan por separado.

**¿Puedo usar mi propio `android.jar`?**
Sí. En **Ajustes del IDE → SDK**, puedes seleccionar cualquier `android.jar` que tengas en tu almacenamiento.

**¿Es necesario el NDK?**
Solo si planeas compilar aplicaciones con código nativo (C/C++). Si solo haces apps Java, puedes omitirlo.

**¿Dónde reporto errores o sugerencias?**
Puedes contactarme en:
- **WhatsApp:** [@DayfoxAnims](https://wa.me/)
- **X (Twitter):** [@dayfoxanims](https://x.com/dayfoxanims)

---

## 📄 Licencia

Este proyecto es de **código cerrado**. Los archivos distribuidos en este repositorio (APK, rootfs, NDK) son para uso personal y no pueden ser modificados ni redistribuidos sin permiso explícito del autor.

---

Hecho con ❤️ por [DayFox](https://x.com/dayfoxanims) 🦊
