# christhz666.github.io

## Editor de Diapositivas de Protección Radiológica

Editor interactivo para las 13 diapositivas del curso de Protección Radiológica, con capacidad de exportación a PowerPoint.

### Características

- **Editor Visual Interactivo**: Arrastra y mueve elementos libremente en cada diapositiva
- **Navegación Intuitiva**: Usa las flechas ← → para navegar entre diapositivas
- **Exportación a PowerPoint**: Genera archivos PPTX editables con un solo clic

### Exportación a PowerPoint

El botón "📊 Exportar a PowerPoint" genera un archivo `Proteccion_Radiologica.pptx` con las siguientes características:

#### Contenido Editable ✅
- **Texto completamente editable**: Todos los títulos y contenidos de texto son objetos nativos de PowerPoint que puedes modificar
- **Formato preservado**: Se mantienen los estilos (fuentes Montserrat y Roboto, colores, tamaños)
- **Estructura organizada**: Los elementos mantienen su posición y jerarquía

#### Gráficos y Diagramas
- Los gráficos Chart.js y elementos visuales complejos se capturan como imágenes PNG de alta calidad
- Se espera 1.5 segundos para que los gráficos se rendericen completamente antes de capturarlos
- Las imágenes mantienen transparencia y se integran con el fondo oscuro

#### Mejoras Implementadas
1. **Solución al problema de editabilidad**: Antes las diapositivas eran imágenes completas (no editables). Ahora el texto es nativo de PowerPoint.
2. **Solución al problema de "modelos no cargan"**: Se aumentó el tiempo de espera para que los gráficos Chart.js se rendericen completamente antes de capturarlos.
3. **Manejo de errores**: Si una diapositiva falla, se muestra un mensaje específico en lugar de detener todo el proceso.

### Uso

1. Abre `index.html` en un navegador moderno
2. Navega por las diapositivas usando las flechas del teclado
3. Arrastra elementos para reposicionarlos (los cambios se guardan automáticamente)
4. Haz clic en "📊 Exportar a PowerPoint" para generar el archivo PPTX
5. Abre el archivo en PowerPoint y edita el texto libremente

### Tecnologías Utilizadas

- **html2canvas**: Captura de elementos visuales complejos
- **PptxGenJS**: Generación de archivos PowerPoint nativos
- **Chart.js**: Renderizado de gráficos en diapositivas 9 y 11
- **Tailwind CSS**: Estilos de las diapositivas
- **Font Awesome**: Iconos decorativos

### Compatibilidad

- Funciona 100% en el cliente (sin necesidad de servidor)
- Compatible con Chrome, Firefox, Safari, Edge (versiones recientes)
- Los archivos PPTX son compatibles con PowerPoint 2016+, Google Slides, LibreOffice Impress