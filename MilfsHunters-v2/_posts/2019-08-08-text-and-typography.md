---
title: Mini Tutorial de GitLab
description: Aprende a usar GitLab para crear repositorios, colaborar y gestionar tus proyectos.
author: Alejandro Avilés Fernández
date: 2025-03-19
categories: [Git, Desarrollo]
tags: [GitLab, Tutorial]
pin: true
math: false
mermaid: false
image:
  path: /ruta/a/imagen.png
  lqip: data:image/webp;base64,....
  alt: GitLab tutorial visual
---

# 🚀 Mini Tutorial de GitLab

GitLab es una plataforma de DevOps que facilita el control de versiones, integración continua (CI) y colaboración en equipo. A continuación, te guiaré a través de los pasos básicos para empezar a usar GitLab.

## 📂 1. Crear un Repositorio en GitLab

1. **Inicia sesión** en [GitLab](https://gitlab.com/).
2. Haz clic en **"New Project"**.
3. Elige **"Create Blank Project"**.
4. Asigna un **nombre** al repositorio, selecciona la **visibilidad** (público o privado) y haz clic en **"Create project"**.

---

## 💻 2. Clonar un Repositorio en Local

Para trabajar con el repositorio en tu máquina, utiliza el siguiente comando:

```bash
git clone https://gitlab.com/usuario/nombre-del-repositorio.git

Luego, navega a la carpeta del repositorio: cd nombre-del-repositorio

## 📝 3. Hacer Cambios y Subirlos

- **Realiza cambios en los archivos** del repositorio.
- **Añade los cambios al área de staging** con el siguiente comando:

```bash
git add .

