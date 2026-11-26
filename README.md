# Parque Residencial Aurora · PBL 3 Ciudad

Sitio web estático preparado para GitHub Pages. No necesita Node, npm ni un proceso de compilación.

## Contenido

- `index.html`: sitio principal con plano de planta interactivo, fichas técnicas, cuatro láminas, cálculos y generador de QR. **Las cinco imágenes utilizadas en las secciones previas a la maqueta 3D están incrustadas dentro del HTML** para evitar errores de rutas o de carpetas al publicar.
- `maqueta-3d.html`: visor Three.js incorporado como sección del sitio y disponible también en pestaña independiente.
- `assets/`: copias originales de las imágenes, conservadas como respaldo y para futuras ediciones.
- `documentos/`: informe revisado con anexo correctivo y cálculo de volúmenes.

## Publicar en GitHub Pages

1. Descarga y descomprime el ZIP.
2. Abre la carpeta descomprimida y selecciona **todo lo que está dentro**: `index.html`, `maqueta-3d.html`, `assets/` y `documentos/`.
3. Sube ese contenido a la **raíz del repositorio**. No subas solamente el archivo HTML ni dejes `index.html` dentro de una carpeta adicional. La estructura debe quedar así:

   ```text
   repositorio/
   ├── index.html
   ├── maqueta-3d.html
   ├── assets/
   └── documentos/
   ```

4. En el repositorio abre **Settings → Pages**.
5. En **Build and deployment**, selecciona **Deploy from a branch**, la rama `main` y la carpeta `/(root)`, y guarda.
6. Abre la URL pública de GitHub Pages. El plano interactivo y las cuatro láminas ya están embebidas en `index.html`; la maqueta 3D y los PDF sí se sirven desde los archivos acompañantes, por lo que esos archivos deben permanecer en la raíz y sus carpetas respectivas.
7. Baja a **Un solo QR para todo el proyecto**, pega la URL pública, pulsa **Generar QR** y luego **Descargar PNG**.

## Comprobación rápida después de publicar

- En la sección **Plano de planta interactivo** debe verse la ilustración completa del parque detrás de los marcadores.
- En **Las cuatro láminas del proyecto** deben aparecer las cuatro previsualizaciones y abrirse al pulsarlas.
- En **Maqueta 3D interactiva** debe cargar el visor. Este depende de Three.js y de tipografías alojadas en CDN, por lo que requiere internet.
- Los enlaces de documentos abren los PDF guardados en `documentos/`.

## Notas técnicas

- La escala lineal es 1:200: 1 m real equivale a 0.5 cm en la maqueta.
- Se conservan los 17 elementos numerados de la leyenda de la lámina 1 y se identifica la fuente ornamental con `F`, separada del tanque `2`.
- Las fichas hidráulicas siguen el anexo técnico correctivo y el documento de cálculo de volúmenes: fuente ornamental y tanque elevado son objetos distintos.
- En el visor 3D se ajustó el radio de las dos superficies de agua de la fuente de 4.62 m a 4.60 m, según la corrección indicada en el anexo.
- El QR utiliza un generador externo. Se genera con la dirección pública real de GitHub Pages, no con una dirección provisional.

## Fuentes incluidas

- `documentos/Informe-Avance2-Parque-Aurora.pdf`
- `documentos/Calculo-de-Volumenes-Parque-Aurora.pdf`
