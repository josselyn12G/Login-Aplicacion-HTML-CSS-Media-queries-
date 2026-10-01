# Login-Aplicacion-HTML-CSS-Media-queries-

Pantalla de inicio de sesión de **AdminExpress**, construida únicamente con HTML y CSS (sin JavaScript ni frameworks). Es una actividad de la materia Ingeniería Web (Semana 2) enfocada en maquetación con Flexbox y diseño responsivo con media queries.

## Vista general

- **Escritorio:** pantalla dividida en dos mitades. A la izquierda, un panel azul con el nombre de la marca; a la derecha, el formulario de acceso.
- **Tablet (≤ 1024px):** se reduce el padding del panel derecho y el botón ocupa todo el ancho.
- **Celular (≤ 768px):** se oculta el panel azul, el formulario pasa a ocupar toda la pantalla, las etiquetas (`label`) se ocultan visualmente (siguen disponibles para lectores de pantalla) y aparece el enlace "Don't have an account? Sign Up".

## Estructura del proyecto

```
Tarea/
├── index.html   # Estructura de la página y formulario
├── styles.css   # Estilos, variables de color y media queries
└── README.md
```

## Tecnologías y recursos

- HTML5 semántico (`main`, `section`, `form`, `label`).
- CSS3: variables personalizadas (`:root`), Flexbox, posicionamiento absoluto para los íconos de los campos, `clamp()` para el título fluido y media queries.
- [Google Sans](https://fonts.google.com/) como tipografía.
- [Material Symbols Outlined](https://fonts.google.com/icons) para los íconos de correo, candado y visibilidad.

## Convenciones

Las clases siguen la metodología **BEM** (por ejemplo `login-section__input-container`), y los colores se definen como variables en `:root` de [styles.css](styles.css).

## Cómo ejecutarlo

No requiere instalación ni compilación:

1. Clona o descarga el repositorio.
2. Abre [index.html](index.html) en cualquier navegador moderno.
3. Para probar el diseño responsivo, redimensiona la ventana o usa las herramientas de desarrollo del navegador (modo dispositivo).

> Se necesita conexión a internet para cargar la tipografía y los íconos desde Google Fonts.

## Limitaciones

- El formulario es solo visual: no tiene lógica de autenticación ni validación más allá de la que ofrece `type="email"`.
- El botón de mostrar/ocultar contraseña y los enlaces "Forgot password?" y "Sign Up" aún no tienen funcionalidad.
