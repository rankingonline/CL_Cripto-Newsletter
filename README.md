# Cripto Newsletter Project

Este proyecto contiene el archivo histórico de las newsletters mensuales.

## Estructura del Proyecto

```
/
├── index.html          # Página principal con acceso a todas las ediciones
├── README.md           # Documentación del proyecto
├── newsletters/        # Carpeta contenedora de las ediciones mensuales
│   └── febrero-2026/   # Edición de Febrero 2026
│       └── index.html  # HTML del correo (código inline)
└── assets/             # Recursos estáticos (imágenes, logos)
    └── febrero-2026/   # Recursos específicos para Febrero 2026
```

## Instrucciones para crear una nueva newsletter

1. Crear una nueva carpeta en `newsletters/` con el nombre del mes (ej. `marzo-2026`).
2. Crear una nueva carpeta en `assets/` con el mismo nombre.
3. Copiar el archivo `index.html` de una edición anterior a la nueva carpeta y actualizar el contenido.
4. Agregar una nueva "card" en el archivo `index.html` raíz vinculando a la nueva edición.

## Visualización


## Paleta de Colores

El diseño se basa en una paleta "Dark Mode" premium para el sector Cripto.

| Color | Hex | Uso |
|-------|-----|-----|
| **Primary** | `#0F1A4E` | Fondo principal, Header, Footer (Deep Blue) |
| **Secondary/Accent** | `#FF6F00` | Botones, Links, Hover effects (Vibrant Orange) |
| **White** | `#FFFFFF` | Texto principal, Títulos |
| **Text Secondary** | `#B0B8D4` | Subtítulos, Texto secundario (Desaturated Blue) |
| **Card Background** | `#16225e` | Fondo de contenedores/tarjetas |

## Criterios de Aceptación para Correos

Para asegurar la compatibilidad y calidad de cada newsletter, se deben cumplir los siguientes criterios antes de su envío:

1.  **Código Inline**: Todo el CSS crítico debe estar inyectado en línea (`style="..."`) para compatibilidad con Gmail.
2.  **Ancho Máximo**: El contenedor principal debe tener un `max-width: 600px` para lectura óptima.
3.  **Compatibilidad Outlook**:
    *   Uso de "Ghost Tables" (comentarios condicionales `<!--[if mso]>...<![endif]-->`) para mantener el ancho en Outlook de escritorio.
    *   Uso de VML para fondos con gradientes si es necesario.
4.  **Imágenes**:
    *   Todas las imágenes deben tener `display: block`.
    *   Deben incluir texto alternativo (`alt`).
5.  **Tipografía**:
    *   Usar fuentes seguras como `Helvetica, Arial, sans-serif` como fallback inmediato de la fuente web (`Outfit`).
6.  **Móvil**:
    *   El diseño debe ser fluido y adaptarse al 100% del ancho en pantallas pequeñas.
    *   Los tamaños de fuente y botones deben ser legibles en móvil (min 14px texto, min 44px altura táctil).
7.  **Dark Mode**:
    *   Incluir meta tags `color-scheme: dark` y `supported-color-schemes: dark`.
    *   El diseño está optimizado nativamente para modo oscuro.
