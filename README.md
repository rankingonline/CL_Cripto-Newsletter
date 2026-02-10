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

Para visualizar la newsletter, simplemente abre el archivo `index.html` de la carpeta correspondiente en tu navegador.
