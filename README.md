


**Página Web Ubicampus**

- **Descripción:** Proyecto de sitio web estático para la guía Ubicampus. Contiene páginas HTML y recursos (imágenes, estilos) usados para la presentación del sitio.

**Estructura del repositorio:**
- `Bienvenida/` : páginas principales (por ejemplo `Inicio.html`, `menu.html`).
- `Enlaces/` : páginas de enlaces por categoría.
- `img/` : recursos gráficos y archivos relacionados.
- `styles.css`, `Bienvenida/styles_menu.css` : estilos globales y específicos.
- `README.md` : este archivo.

**Cómo ver el sitio localmente**
- Opción rápida: abrir `Bienvenida/Inicio.html` directamente en el navegador.
- Opción con servidor local (recomendada para rutas y recursos): en PowerShell, desde la raíz del repositorio ejecutar:

```
python -m http.server 8000
```

Luego abrir en el navegador: `http://localhost:8000/Bienvenida/Inicio.html`.

**Navegar al repositorio con `cd` (PowerShell)**
- Desde PowerShell, mueve la terminal a la carpeta del repositorio usando `cd` (o `Set-Location`). Ejemplos:

	- Ruta absoluta (ajusta según tu usuario):

	```powershell
	cd C:\Users\hazie\Documents\GitHub\Pagina-Web-Ubicampus_
	```

	- Si ya estás en `GitHub` o una carpeta superior, usa ruta relativa:

	```powershell
	cd Pagina-Web-Ubicampus_
	```

	- Para ir directamente a la carpeta de la página de bienvenida:

	```powershell
	cd Pagina-Web-Ubicampus_\Bienvenida
	```

- Notas rápidas:
	- Si la ruta contiene espacios, envuélvela entre comillas: `cd "C:\Ruta con espacios\Proyecto"`.
	- `Set-Location` es equivalente a `cd` en PowerShell: `Set-Location C:\ruta\al\repositorio`.

Después de posicionarte en la raíz del repositorio puedes ejecutar el servidor local:

```powershell
python -m http.server 8000
```

Y abrir `http://localhost:8000/Bienvenida/Inicio.html` en el navegador.

**Contribuciones**
- Hacer fork, crear una rama, realizar cambios y abrir un Pull Request.
- Para cambios menores (texto/estilos) puedes editar los archivos HTML/CSS directamente.

**Créditos y activos**
- Las imágenes y archivos en `img/` pertenecen al autor o a su origen indicado en los archivos.

**Licencia**
- Sin licencia especificada. Contactar al autor si desea aplicar una licencia.

**Autor / Contacto**
- Repositorio: `HazielHc/Pagina-Web-Ubicampus_` (usuario: `HazielHc`).

Si quieres, puedo:
- Añadir una licencia (por ejemplo MIT).
- Crear un `index.html` que redirija a `Bienvenida/Inicio.html`.

