---
layout: post
title:  "Cómo desplegar un sitio Jekyll en GitHub Pages"
date:   2025-03-12 
categories: jekyll deployment github
---

En este post, te explicaré cómo desplegar tu sitio Jekyll en **GitHub Pages** para que puedas compartirlo con el mundo. GitHub Pages es un servicio gratuito que te permite alojar sitios web directamente desde un repositorio de GitHub. Aquí tienes los pasos básicos para poner en marcha tu propio sitio en GitHub Pages.

## 1. Prepara tu sitio Jekyll

Antes de comenzar, asegúrate de tener un sitio Jekyll listo para ser desplegado. Si aún no lo tienes, puedes crear uno usando el siguiente comando:

```bash
jekyll new mi-sitio
cd mi-sitio
```

## 2. Crea un repositorio en GitHub

Dirígete a GitHub y crea un nuevo repositorio. Si deseas que el sitio esté en tu dominio personal (por ejemplo, https://username.github.io), el nombre del repositorio debe seguir este formato:

username.github.io

Asegúrate de inicializar el repositorio con un archivo README.md si lo deseas.

## 3. Conecta tu sitio local con el repositorio de GitHub

Abre una terminal y navega hasta la carpeta de tu sitio Jekyll. Luego, inicializa un repositorio Git y vincúlalo con tu repositorio en GitHub:

```bash
git init
git remote add origin https://github.com/tu-usuario/mi-repositorio.git
```

## 4. Realiza el primer commit

Ahora, realiza el primer commit y sube los archivos de tu sitio a GitHub:

```bash
git add .
git commit -m "Primer commit para GitHub Pages"
git push -u origin main
```

## 5. Habilita GitHub Pages

Ve a la configuración de tu repositorio en GitHub. En la sección GitHub Pages, selecciona la rama que deseas desplegar. Si tu sitio está en la rama main, selecciona esa opción. Si estás utilizando otra rama, también puedes seleccionarla.

## 6. Accede a tu sitio

Una vez que el proceso haya finalizado, tu sitio estará disponible en la siguiente URL:

https://tu-usuario.github.io/mi-repositorio

## 7. Personalización

Cuando este todo listo, puedes personalizar tu sitio modificando los archivos proporcionados en la base de Jekyll, y agregando nuevas páginas y entradas. 


## Conclusión

¡Y eso es todo! Ahora tienes tu sitio Jekyll desplegado en GitHub Pages y listo para compartirlo con el mundo.

Espero que esta guía sobre cómo desplegar tu sitio Jekyll en GitHub Pages te haya sido útil. Si tienes alguna pregunta o necesitas ayuda adicional, no dudes en dejar un comentario o revisar la documentación oficial de Jekyll y GitHub Pages. ¡El mundo de la web está al alcance de tu mano!

Recuerda que con un poco de práctica, podrás personalizar y mejorar tu sitio a tu gusto, y compartirlo fácilmente con todos. ¡Mucho éxito con tu proyecto web y feliz codificación!