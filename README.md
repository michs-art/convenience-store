## 📋 Primeros pasos
-Buscar que es un json
-Que es un object
-Que es un Array

-Como configurar que la carpeta app/ sea la principal en nuxt3
-Como trabajar con arrays (.map, .filer, .find, .forEach, for())


# 🛒 Tienda en Línea de Productos de Conveniencia

Una aplicación web moderna para gestionar y vender productos de conveniencia. Construida con **Nuxt 3**, **Vue 3** y **Tailwind CSS**.

## 📋 Descripción del Proyecto

Este proyecto es una práctica de desarrollo web que implementa una tienda en línea completa con funcionalidades de e-commerce. Los productos se organizan en una estructura de datos flexible que soporta imágenes, precios, inventario y fechas de caducidad.

## 🛠️ Stack Tecnológico

- **Framework**: Nuxt 3 + Vue 3
- **Estilos**: Tailwind CSS
- **Lenguaje**: TypeScript
- **Runtime**: Node.js

## 📦 Estructura de Datos

### Esquema de Producto

Los productos se almacenan como objetos dentro de un array:

```json
[
  {
    "_id": "ID único del producto",
    "product": "Nombre del producto",
    "price": 99.99,
    "picture": "URL de la imagen principal",
    "created_at": "2024-01-15T10:30:00Z",
    "updated_at": "2024-01-20T14:45:00Z",
    "count": 50,
    "description": "Descripción breve del producto (opcional)",
    "expiration": "2025-12-31T23:59:59Z",
    "isExpiry": true,
    "collage": ["url1.jpg", "url2.jpg", "url3.jpg"]
  }
]
```

**Campos:**
- `_id` (string): Identificador único del producto
- `product` (string): Nombre del producto
- `price` (number): Precio en unidad monetaria
- `picture` (string): URL de la imagen principal
- `created_at` (string - ISO): Fecha de creación
- `updated_at` (string - ISO): Última modificación
- `count` (number): Cantidad disponible en inventario
- `description` (string - opcional): Breve descripción
- `expiration` (string - ISO): Fecha de caducidad (solo si `isExpiry` es true)
- `isExpiry` (boolean): Indica si el producto caduca
- `collage` (array): Galería de imágenes del producto

## 🎨 Diseño y Maquetación

- [ ] Configurar Tailwind CSS con utilidades personalizadas
- [ ] Implementar sistema de componentes reutilizables
- [ ] Diseño responsive para escritorio, tablet y móvil

## 📄 Vistas Principales

El proyecto incluirá las siguientes páginas:

- **Página Principal**: Inicio con eslóganes, productos destacados, ofertas y redes sociales
- **Catálogo**: Listado completo de productos con filtros
- **Búsqueda**: Búsqueda avanzada de productos
- **Productos Populares**: Sección dedicada a los artículos más vendidos
- **Carrito de Compras**: Gestión del carrito y checkout
- **Autenticación**: Inicio de sesión y registro de usuarios
- **Perfil de Usuario**: Historial de compras y gestión de cuenta
- **Página de Producto**: Detalle completo del artículo

## 🚀 Características Planeadas

- [ ] Catálogo de productos con búsqueda y filtros
- [ ] Sistema de carrito de compras
- [ ] Autenticación de usuarios (login/registro)
- [ ] Historial de compras por usuario
- [ ] Gestión de inventario
- [ ] Manejo de productos con fecha de caducidad
- [ ] Galería de imágenes por producto
- [ ] Sistema de puntuación y reseñas (considerando)
- [ ] Integración de métodos de pago (considerando)

## 📦 Instalación

```bash
# Clonar el repositorio
git clone <repo-url>

# Instalar dependencias
npm install

# Ejecutar en modo desarrollo
npm run dev

# Compilar para producción
npm run build
```

## 📱 Estructura del Proyecto

```
convenience-store/
├── app/
│   ├── assets/       # Recursos estáticos (CSS, imágenes)
│   ├── components/   # Componentes reutilizables de Vue
│   └── pages/        # Páginas de la aplicación
├── server/           # Lógica del servidor
├── nuxt.config.ts    # Configuración de Nuxt
├── tsconfig.json     # Configuración de TypeScript
└── package.json      # Dependencias del proyecto
```

## 📝 Notas de Desarrollo

- Recordar configurar Tailwind CSS correctamente antes de maquetar
- Mantener la estructura de datos consistente en toda la aplicación
- Implementar validaciones en el lado del cliente y servidor
- Considerar la accesibilidad (WCAG) en el diseño

## 📄 Licencia

Este proyecto es una práctica educativa.

