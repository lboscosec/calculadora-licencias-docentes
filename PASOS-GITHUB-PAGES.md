# Pasos para publicar en GitHub Pages

## 1. Crear cuenta en GitHub

Si no tenés, andá a [github.com](https://github.com) y creala.

## 2. Crear un nuevo repositorio

- Andá a [github.com/new](https://github.com/new).
- Nombre del repositorio: `calculadora-licencias-docentes` (o el que prefieras).
- Marcá **Public**.
- No agregues README ni .gitignore porque ya los tenés listos.
- Hacé clic en **Create repository**.

## 3. Subir los archivos

Desde tu computadora, en la carpeta del proyecto, ejecutá estos comandos en la terminal:

```bash
git init
git add .
git commit -m "Primera versión: calculadora PBA y CABA"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/calculadora-licencias-docentes.git
git push -u origin main
```

Reemplazá `TU_USUARIO` por tu nombre de usuario de GitHub.

## 4. Activar GitHub Pages

- Dentro del repo, andá a **Settings**.
- En el menú lateral, hacé clic en **Pages**.
- En **Source**, seleccioná **Deploy from a branch**.
- Seleccioná **Branch: main** y **Folder: / (root)**.
- Hacé clic en **Save**.

## 5. Esperar y probar

En unos minutos, GitHub Pages va a publicar el sitio. El link va a ser:

```
https://TU_USUARIO.github.io/calculadora-licencias-docentes
```

## 6. Actualizar el link de Cafecito

Antes de compartirlo, abrí `index.html` y reemplazá:

```html
https://cafecito.app/tuusuario
```

por tu link real de Cafecito.

## 7. Compartir

Ya podés compartir el link en redes, grupos de WhatsApp, etc.

---

## ¿Y si quiero un dominio propio?

En **Settings → Pages** podés agregar un dominio personalizado (por ejemplo `tusitio.com.ar`). GitHub te va a indicar qué registros DNS configurar.
