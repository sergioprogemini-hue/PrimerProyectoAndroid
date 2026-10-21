# Mi Primer Proyecto Android

Proyecto desarrollado para el curso **Fundamentos de Desarrollo de Aplicaciones Móviles con Android** de la Universidad Nacional Autónoma de México (UNAM) en Coursera.

**Autor:** Sergio Esteban Garay Lee  

---

## 📋 Descripción del Proyecto
Esta aplicación Android demuestra los conceptos fundamentales de:
1. **Internacionalización y localización (i18n):** Soporte completo para cuatro idiomas distintos.
2. **Gráficos redimensionables:** Implementación de un fondo con formato **Nine-Patch (`.9.png`)** que se adapta a cualquier tamaño de pantalla sin distorsionar el logotipo central de Android.
3. **Diseño adaptable y responsivo:** Soporte para múltiples resoluciones, tamaños de pantalla (teléfonos y tablets) y cambios de orientación (Vertical / Portrait y Horizontal / Landscape).

---

## ✅ Cumplimiento de Criterios de Evaluación

### 1. Soporte para Cuatro Idiomas
El proyecto cuenta con sus respectivos directorios y archivos de recursos en `app/src/main/res/`:
* **Español (Idioma por defecto):** `res/values/strings.xml`
  * Título: *Bienvenido*
  * Botón: *Entrar*
* **Inglés:** `res/values-en/strings.xml`
  * Título: *Welcome*
  * Botón: *Enter*
* **Francés:** `res/values-fr/strings.xml`
  * Título: *Bienvenue*
  * Botón: *Entrer*
* **Alemán:** `res/values-de/strings.xml`
  * Título: *Willkommen*
  * Botón: *Betreten*

### 2. Imagen de Fondo Nine-Patch (.9.png)
* Archivo ubicado en: `app/src/main/res/drawable/fondo.9.png`
* **Zonas de estiramiento:** Las guías de 1 píxel (borde superior e izquierdo) fueron configuradas específicamente para permitir la expansión vertical en el cielo azul y la expansión horizontal a los costados de las nubes, dejando intacta el área central del marcianito de Android para evitar que se deforme.

### 3. Soporte para Múltiples Pantallas y Orientaciones
* **Orientación Vertical (Portrait):** `app/src/main/res/layout/activity_main.xml`
* **Orientación Horizontal (Landscape):** `app/src/main/res/layout-land/activity_main.xml`
* Los componentes (`TextView` y `Button`) se encuentran centrados y adaptados con unidades independientes de la densidad (`dp` y `sp`) para garantizar una visualización perfecta en cualquier dispositivo.

---

## 📁 Estructura del Repositorio

```text
PrimerProyectoAndroid/
├── app/
│   ├── build.gradle
│   └── src/
│       └── main/
│           ├── AndroidManifest.xml
│           ├── java/com/example/miprimerproyecto/
│           │   └── MainActivity.java
│           └── res/
│               ├── drawable/
│               │   └── fondo.9.png
│               ├── layout/
│               │   └── activity_main.xml
│               ├── layout-land/
│               │   └── activity_main.xml
│               ├── values/
│               │   └── strings.xml
│               ├── values-en/
│               │   └── strings.xml
│               ├── values-fr/
│               │   └── strings.xml
│               └── values-de/
│                   └── strings.xml
├── build.gradle
├── settings.gradle
└── README.md
```
