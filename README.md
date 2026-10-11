# Sitio web de ALIPE

Sitio inicial en español para ALIPE, asociación de pastores latinos dentro de la Evangelical Covenant Church. HTML y CSS simples: no requiere dependencias, framework ni compilación.

## Archivos

- `public/index.html`: Inicio, Acerca de ALIPE, Noticias, Eventos y Contacto.
- `public/noticias/index.html`: página de noticias.
- `public/assets/styles.css`: estilos compartidos y adaptación a pantallas pequeñas.
- `AGENTS.md`: instrucciones para futuras tareas de código.

Todos los archivos desplegables están en `public/`. La documentación no se publica.

## Cloudflare Pages

Conectar el repositorio `ALIPEUSA/alipe-website` y configurar:

| Ajuste | Valor |
| --- | --- |
| Rama de producción | `main` |
| Framework | Ninguno |
| Comando de compilación | Vacío (sin comando) |
| Directorio de salida | `public` |
| Directorio raíz | Raíz del repositorio |

Estos son los ajustes a introducir en Cloudflare Pages; este repositorio no configura la cuenta ni crea el proyecto de hosting. Revisar la vista previa del pull request antes de fusionarlo manualmente.

## Editar y revisar

1. Actualizar `main` desde el remoto y crear una rama para cada cambio. Nunca hacer commits directamente en `main`.
2. Editar el HTML correspondiente o el CSS compartido. Mantener el español, `lang="es"`, los títulos jerárquicos, las etiquetas de navegación y el enlace para saltar al contenido.
3. Reemplazar los marcadores **Información pendiente** solo con datos confirmados y autorizados. No inventar información ni añadir imágenes copiadas de otras páginas.
4. Para una vista previa local, ejecutar `python3 -m http.server 8000 --directory public` desde la raíz y abrir `http://localhost:8000/` y `http://localhost:8000/noticias/`. Usar un servidor: las rutas parten de la raíz del sitio.
5. Revisar los enlaces y sus destinos, el foco y la navegación con teclado, y el diseño en escritorio y móvil. Ejecutar `git diff --check`.
6. Hacer commit en la rama, publicarla y abrir un pull request a `main`, con resultados de validación y datos pendientes. No fusionarlo automáticamente.

Para publicar una noticia, sustituir el marcador de la página de noticias por contenido aprobado con título, texto y fecha confirmada; actualizar también el resumen de Noticias en Inicio. Mantener las rutas existentes y comprobar los enlaces si se añaden páginas.

## Información pendiente

- Presentación oficial, misión e historia de ALIPE.
- Noticias: títulos, contenido y fechas de publicación confirmadas.
- Eventos: detalles, fechas, horarios, lugares e información de participación.
- Medio de contacto oficial autorizado.

No se han añadido dirigentes, datos de contacto ficticios, fechas de eventos, enlaces de donaciones ni imágenes.
