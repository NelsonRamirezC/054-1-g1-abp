# Proyecto: Banco Digital Alky-Wallet

Descripción
-----------
Interfaz web estática para operaciones bancarias básicas: inicio de sesión, depósito y visualización de transacciones. Está pensada como una aplicación front-end educativa o de demostración, usando HTML, CSS y JavaScript sin backend persistente.

## Características
---------------
- Páginas principales: [index.html](index.html), [login.html](login.html), [deposit.html](deposit.html), [transactions.html](transactions.html).
- Manejo de interacción cliente: scripts en `assets/js/` para login, depósitos y listado de transacciones.
- Estilos centralizados en `assets/css/style.css`.
- Arquitectura estática fácil de desplegar en GitHub Pages u otro hosting de archivos estáticos.

## Estructura del proyecto
-----------------------
- `index.html` — Página de inicio.
- `login.html` — Formulario de autenticación (demo).
- `deposit.html` — Formulario para realizar depósitos.
- `transactions.html` — Visualiza transacciones (fragmentos y lógica JS).
- `assets/css/style.css` — Estilos globales.
- `assets/js/login.js` — Lógica de autenticación (front-end).
- `assets/js/deposit.js` — Lógica para depósitos.
- `assets/js/transactions.js` y `assets/js/transactions.fragment.js` — Listado y fragmentos de la vista de transacciones.

## Instalación y ejecución (desarrollo)
----------------------------------
1. Requisitos: un navegador moderno. Para servir los archivos localmente se recomienda usar un servidor HTTP simple / alternativa usar Live Server

Opcional: con Python 3 instalado, desde la raíz del proyecto ejecutar:

```bash
python -m http.server 8000
# o
python3 -m http.server 8000
```

Abrir `http://localhost:8000` en el navegador.

## Uso
---
- Abrir [index.html](index.html) para navegar por la aplicación.
- Ir a [login.html](login.html) para simular autenticación.
- Usar [deposit.html](deposit.html) para probar la interfaz de ingreso de fondos.
- Consultar [transactions.html](transactions.html) para ver el historial (simulado por front-end).

## Notas de desarrollo
-------------------
- La aplicación es completamente estática: no hay persistencia segura ni API real.
- Para pruebas rápidas, los datos se mantienen en memoria (JavaScript) o en el almacenamiento del navegador según la implementación actual.
- Recomiendo revisar los archivos en `assets/js/` para adaptar lógica y validaciones.

## Buenas prácticas y consideraciones
---------------------------------
- No usar este proyecto en producción con datos reales ni credenciales sensibles.
- Validar entradas en el cliente y, si se añade backend, también validar en servidor.
- Añadir linting (ESLint) y formateo (Prettier) si se extiende el proyecto.
- Incluir pruebas unitarias para la lógica de negocio si se mueve la lógica a módulos reutilizables.
- Asegurar accesibilidad: etiquetas `label`, roles ARIA y navegación por teclado.

## Despliegue
---------
- Al ser un sitio estático, se puede desplegar en GitHub Pages: crear/usar la rama `gh-pages` o configurar Pages desde `main` con la carpeta raíz.
- También sirve en cualquier hosting estático (Netlify, Vercel, S3 + CloudFront, etc.).

## Contribuciones
--------------
1. Fork del repositorio.
2. Crear una rama descriptiva: `feature/nombre` o `fix/descripcion`.
3. Abrir pull request describiendo cambios.

## Licencia
--------
Este proyecto puede licenciarse bajo MIT (o la licencia que prefieras). Añade un archivo `LICENSE` si decides publicar bajo una licencia específica.

## Contacto
-------
Para preguntas o mejoras, abre un issue en el repositorio o contacta al mantenedor.

