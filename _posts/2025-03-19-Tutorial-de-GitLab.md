---
title: Mini Tutorial de GitLab
description: Aprende a usar GitLab para crear repositorios, colaborar y gestionar tus proyectos.
author: aaf925
date: 2025-03-19
categories: [Git, Desarrollo]
tags: [GitLab, Tutorial]
pin: true
math: false
mermaid: false
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

1. **git bash**
git clone https://gitlab.com/usuario/nombre-del-repositorio.git

2. Luego, navega a la carpeta del repositorio: cd nombre-del-repositorio

## 📝 3. Hacer Cambios y Subirlos

- **Realiza cambios en los archivos** del repositorio.
- **Añade los cambios al área de staging** con el siguiente comando:

**git bash**
git add .

1. Confirma los cambios con un mensaje descriptivo:
**git commit** -m "Descripción del cambio"
2. Sube los cambios al repositorio remoto para actualizarlo:
git push origin main

## 🔄 4. Crear una Rama y Fusionar

1. **Crear una nueva rama con el siguiente comando:**
git checkout -b nombre-de-la-rama

2. **Subir la nueva rama al repositorio remoto:**
git push origin nombre-de-la-rama

3. Crear un Merge Request (MR) en GitLab:
4. Ve a la pestaña "Merge Requests" en GitLab.
5. Haz clic en "New Merge Request".
6. Selecciona las ramas origen y destino (por ejemplo, main o la rama correspondiente).
7. Haz clic en "Create merge request" para completar el proceso.