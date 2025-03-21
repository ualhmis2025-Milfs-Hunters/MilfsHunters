---
title: Instalación de Jekyll
author: anm020
date: 2025-03-20
categories: [Tutorial]
tags: [writing]
render_with_liquid: false
---

# Instalación y Configuración básica de Jekyll

## Requisitos previos

Antes de instalar Jekyll, asegúrate de tener los siguientes requisitos en tu sistema:

- **Ruby** (versión 2.5.0 o superior)
- **RubyGems**
- **GCC y Make** (para compilar extensiones nativas)

Puedes verificar la versión de Ruby instalada con el siguiente comando:

```powershell
ruby -v
```

Si no tienes Ruby instalado, puedes hacerlo mediante:

- **Ubuntu/Debian:**
  ```sh
  sudo apt update && sudo apt install ruby-full build-essential zlib1g-dev
  ```
- **MacOS (usando Homebrew):**
  ```sh
  brew install ruby
  ```
- **Windows (usando Chocolatey):**
  ```sh
  choco install ruby -y
  ```

  Después de la instalación, asegúrate de agregar Ruby al `PATH` reiniciando la sesión de PowerShell.


## Instalación de Jekyll

Una vez que tengas Ruby instalado, puedes proceder a instalar Jekyll y Bundler ejecutando:

```powershell
gem install jekyll bundler
```

Verifica que Jekyll se ha instalado correctamente con:

```powershell
jekyll -v
```

## Creación de un nuevo sitio
Para crear un nuevo sitio en Jekyll, usa el siguiente comando:

```powershell
jekyll new mi-sitio
```

Este comando generará una estructura de carpetas y archivos esenciales para tu sitio Jekyll.

## Configuración Básica
Dentro del directorio del sitio recién creado, hay un archivo llamado `_config.yml`. Aquí puedes realizar configuraciones básicas, como cambiar el título del sitio, la descripción y otros parámetros importantes. Un ejemplo de configuración sería:

```yaml
title: "Mi Blog en Jekyll"
author: "Tu Nombre"
description: "Un blog generado con Jekyll."
baseurl: ""
url: "http://tusitio.com"
```

## Ejecutar el Servidor Local
Para previsualizar tu sitio localmente, navega al directorio del sitio y ejecuta:

```powershell
cd mi-sitio
bundle exec jekyll serve
```

Esto iniciará un servidor en `http://localhost:4000/`, donde podrás ver tu sitio en acción.

## Conclusión
Jekyll es una excelente opción para generar sitios estáticos de manera rápida y eficiente. Con esta guía, has aprendido cómo instalarlo, configurarlo y ejecutarlo localmente en Windows usando PowerShell. ¡Ahora puedes comenzar a personalizar tu sitio!

