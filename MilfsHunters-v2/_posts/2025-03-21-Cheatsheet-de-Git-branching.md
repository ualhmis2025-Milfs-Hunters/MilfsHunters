---
layout: post
author : jgm847
title: "Git Branching Cheatsheet"
date: 2025-03-21
categories: [git, cheatsheet]
tags: [git, branching, version-control]
---

# 🧪 Git Branching Cheatsheet

Una referencia rápida para trabajar con ramas en Git. Ideal para cuando necesitas moverte entre ramas, crear nuevas o fusionarlas rápidamente.

---

## 📋 Crear ramas

```bash
# Crear una nueva rama (sin cambiar a ella)
git branch nombre-de-la-rama

# Crear una nueva rama y cambiarse a ella
git checkout -b nombre-de-la-rama

# Crear una nueva rama a partir de otra existente
git checkout -b nueva-rama origen/rama-base
```

---

## 🔄 Cambiar entre ramas

```bash
# Cambiar de rama
git checkout nombre-de-la-rama

# Mostrar todas las ramas locales
git branch

# Mostrar todas las ramas (locales + remotas)
git branch -a
```

---

## 🗑️ Borrar ramas

```bash
# Eliminar una rama local (si ya fue fusionada)
git branch -d nombre-de-la-rama        # Si ya fue fusionada
git branch -D nombre-de-la-rama        # Forzar borrado

# Eliminar una rama del repositorio remoto
git push origin --delete nombre-de-la-rama
```

---

## 🚀 Subir ramas al repositorio remoto

```bash
# Publicar una nueva rama al repositorio remoto y configurarla para hacer push
git push -u origin nombre-de-la-rama
```

---

## 🔁 Fusionar ramas (merge)

```bash
# Integrar cambios de otra rama en la actual
git merge nombre-de-la-rama

# Fusionar sin crear un commit automático
git merge --no-commit nombre-de-la-rama
```

---

## 🧠 Rebase

```bash
# Mover commits actuales para que partan desde otra rama (rebase)
git rebase nombre-de-la-rama

# Interactivo (para reorganizar, editar, etc.)
git rebase -i HEAD~3
```

---

## 🧭 Comparar ramas

```bash
# Mostrar los cambios entre dos ramas
git diff rama1..rama2

# Ver los commits en una rama que no están en otra
git log rama1..rama2
```

---

## 🧼 Limpieza

```bash
# Limpiar ramas remotas eliminadas del listado local
git remote prune origin
```

---

## 🔍 Tips extra

```bash
# Cambiar el nombre de una rama local
git branch -m nuevo-nombre

# Mostrar en qué rama estás actualmente
git branch --show-current

# Establecer la rama remota por defecto para hacer push
git push --set-upstream origin nombre-de-la-rama
```

---

# 🧰 Comandos generales de Git

Una recopilación más extensa de comandos útiles en Git, desde lo básico hasta herramientas avanzadas.

## 🔧 Configuración inicial

```bash
# Configuración de usuario y validación
# Configurar nombre de usuario
git config --global user.name "Tu Nombre"

# Configurar correo electrónico
git config --global user.email "tu@email.com"

# Ver configuración actual
git config --list
```

## 📁 Repositorios

```bash
# Inicialización y clonación de repositorios
# Inicializar un repositorio
git init

# Clonar un repositorio
git clone https://github.com/usuario/repositorio.git

# Ver el estado de los archivos
git status
```

## 📝 Commits

```bash
# Agregar archivos y registrar cambios
# Añadir archivos al staging area
git add archivo.txt
git add .        # Todos los archivos

# Realizar un commit
git commit -m "Mensaje del commit"

# Añadir y commitear de una vez
git commit -am "Mensaje del commit"

# Modificar el último commit
git commit --amend
```

## 🕰️ Historial

```bash
# Consultar historial de commits
# Ver historial de commits
git log

# Ver historial en una línea por commit
git log --oneline

# Ver historial con gráficas
git log --graph --oneline --all
```

## 🔄 Sincronización remota

```bash
# Manejo de orígenes remotos y sincronización
# Ver remotos configurados
git remote -v

# Añadir un remoto
git remote add origin https://github.com/usuario/repositorio.git

# Obtener cambios del remoto
git fetch

# Descargar y fusionar cambios remotos
git pull

# Subir cambios al remoto
git push
```

## 🧪 Stash (guardar cambios sin hacer commit)

```bash
# Guardar y recuperar cambios temporales
# Guardar cambios sin commitear
git stash

# Ver lista de stashes
git stash list

# Aplicar el último stash
git stash apply

# Aplicar y borrar el stash
git stash pop
```

## 🧼 Limpieza

```bash
# Eliminar archivos no versionados
git clean -f

# Eliminar archivos ignorados también
git clean -fdX
```

## 🔍 Buscar

```bash
# Buscar una palabra o patrón en el repo
git grep "texto_a_buscar"
```

## 🧳 Submódulos

```bash
# Administración de submódulos
# Añadir submódulo
git submodule add https://github.com/usuario/proyecto

# Inicializar y clonar submódulos
git submodule update --init --recursive
```

## 🧪 Herramientas de diagnóstico

```bash
# Inspección de cambios y autores
# Ver diferencias entre commits o ramas
git diff

# Ver quién cambió cada línea de un archivo
git blame archivo.txt

# Ver conflictos de fusión
git status
```

---

## 📚 Recursos recomendados

- [Pro Git Book](https://git-scm.com/book/en/v2)
- [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)

---

Con estos comandos tienes un arsenal completo para enfrentar la mayoría de los desafíos con Git. 🚀