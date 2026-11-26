# Parque Residencial Aurora · PBL 3 Ciudad

Sitio web estático preparado para GitHub Pages. No necesita Node, npm ni un proceso de compilación.

## Contenido

- `index.html`: sitio principal con plano de planta interactivo, fichas técnicas, las cuatro láminas, cálculos y sección de QR.
- `maqueta-3d.html`: visor Three.js incorporado como sección del sitio y disponible también en pestaña independiente.
- `assets/`: imágenes de las cuatro láminas y recorte de plano usado para los marcadores interactivos.
- `documentos/`: informe revisado con anexo correctivo y cálculo de volúmenes.

## Publicar en GitHub Pages

1. Crea un repositorio en GitHub, por ejemplo `parque-aurora-pbl3`.
2. Descomprime este ZIP y sube **todo el contenido de esta carpeta** a la raíz del repositorio. `index.html` debe quedar directamente en la raíz, no dentro de otra subcarpeta.
3. En el repositorio abre **Settings → Pages**.
4. En **Build and deployment**, selecciona **Deploy from a branch**; elige la rama `main` y la carpeta `/ (root)`, y guarda.
5. Cuando GitHub Pages muestre la dirección pública, abre esa URL.
6. Baja a **Un solo QR para todo el proyecto**, verifica que aparezca la URL, pulsa **Generar QR** y luego **Descargar PNG**. Ese único QR abre el sitio principal con todos los apartados.

La URL pública es asignada por GitHub Pages al repositorio; por eso el QR no se fija de antemano. La sección de QR lo genera con la dirección real después de publicar.

## Notas técnicas

- La escala lineal es 1:200: 1 m real equivale a 0.5 cm en la maqueta.
- Se conservan los 17 elementos numerados de la leyenda de la lámina 1 y se identifica la fuente ornamental con `F`, separada del tanque `2`.
- Las fichas hidráulicas siguen el anexo técnico correctivo y el documento de cálculo de volúmenes: fuente ornamental y tanque elevado son objetos distintos.
- En el visor 3D se ajustó el radio de las dos superficies de agua de la fuente de 4.62 m a 4.60 m, según la corrección indicada en el anexo.
- El visor 3D carga Three.js y tipografías desde CDN; necesita conexión a internet para cargar todos sus componentes.
- El QR usa un generador externo de códigos QR. La URL introducida es la dirección pública de este sitio.

## Fuentes incluidas

- `documentos/Informe-Avance2-Parque-Aurora.pdf`
- `documentos/Calculo-de-Volumenes-Parque-Aurora.pdf`
