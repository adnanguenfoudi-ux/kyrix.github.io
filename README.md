# KYRIX STORE 🛒

Una tienda en línea moderna y futurista construida con HTML, CSS y JavaScript puro. Caracterizada por su diseño glassmorphism, animaciones suaves y integración completa con PayPal.

![KYRIX STORE](https://adnanguenfoudi-ux.github.io/kyrix.github.io/)

## ✨ Características Principales

### 🎨 Diseño Moderno
- **Glassmorphism**: Efectos de vidrio translúcido con blur
- **Animaciones Suaves**: Transiciones fluidas y micro-interacciones
- **Responsive Design**: Optimizado para todos los dispositivos
- **Tema Oscuro**: Gradientes futuristas y colores vibrantes

### 🛒 Funcionalidades de E-commerce
- **Carrito de Compras**: Agregar, eliminar y modificar cantidades
- **Guardado Automático**: Carrito persiste entre sesiones
- **Sincronización**: Funciona entre pestañas del navegador
- **12 Productos**: Electrónicos y gadgets premium

### 💳 Integración de Pagos
- **PayPal Checkout**: Pagos seguros y confiables
- **Botón Inteligente**: Se adapta al contenido del carrito
- **Confirmación Inmediata**: Feedback visual de transacciones
- **Informes de Pedidos**: Detalles completos de compras

### 📱 Experiencia de Usuario
- **Navegación Fluida**: Scroll suave y navegación intuitiva
- **Notificaciones**: Feedback visual para todas las acciones
- **Formulario de Contacto**: Validación y envío simulado
- **Newsletter**: Suscripción a actualizaciones
- **Botón "Volver Arriba"**: Navegación rápida

## 🚀 Secciones

1. **Hero Section**: Presentación con animaciones de entrada
2. **Productos**: Grid responsive con 12 productos
3. **About**: Información de la empresa y características
4. **Contact**: Formulario de contacto y información
5. **Footer**: Enlaces, newsletter y redes sociales

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura semántica
- **CSS3**: Animaciones, flexbox, grid, glassmorphism
- **JavaScript (Vanilla)**: Interactividad y lógica de negocio
- **PayPal SDK**: Procesamiento de pagos
- **Font Awesome**: Iconos vectoriales
- **Google Fonts**: Tipografía Roboto

## 📦 Instalación y Uso

### Opción 1: GitHub Pages (Recomendado)
La tienda está desplegada automáticamente en:
```
https://adnanguenfoudi-ux.github.io/kyrix.github.io/
```

### Opción 2: Local
```bash
# Clonar el repositorio
git clone https://github.com/adnanguenfoudi-ux.github.io.git

# Abrir index.html en el navegador
# O usar un servidor local
python -m http.server 8000
```

## ⚙️ Configuración de PayPal

Para activar los pagos reales:

1. Ve a [PayPal Developer](https://developer.paypal.com)
2. Crea una aplicación en "Sandbox" o "Live"
3. Copia tu Client ID
4. Reemplaza `YOUR_PAYPAL_CLIENT_ID` en `index.html` línea 625

```html
<script src="https://www.paypal.com/sdk/js?client-id=TU_CLIENT_ID_AQUI&currency=USD"></script>
```

## 📱 Características Responsive

- **Desktop**: Layout completo con grid de 4 columnas
- **Tablet**: Ajustes en espaciado y navegación
- **Mobile**: Diseño de una columna, navegación simplificada

## 🎯 Optimizaciones de Performance

- **Lazy Loading**: Animaciones solo cuando son visibles
- **Debounced Events**: Optimización de eventos de scroll
- **Minimal CSS**: Estilos eficientes sin frameworks
- **Local Storage**: Persistencia sin base de datos

## 🔧 Personalización

### Colores
Los colores principales se definen en las variables CSS:
```css
:root {
  --primary: #00d4ff;
  --secondary: #0099cc;
  --background: linear-gradient(135deg, #0a0a0a 0%, #1a1a2e 50%, #16213e 100%);
}
```

### Productos
Para agregar productos, modifica la sección de productos en `index.html`:
```html
<div class="product-card glass">
    <div class="product-image">
        <i class="fas fa-tu-icono"></i>
    </div>
    <h3 class="product-title">Nombre del Producto</h3>
    <p class="product-price">$99.99</p>
    <button class="add-to-cart" onclick="addToCart('Nombre del Producto', 99.99)">Add to Cart</button>
</div>
```

## 📊 Analytics y Métricas

La tienda incluye:
- Seguimiento de interacciones del usuario
- Console logs para debugging
- Información de pedidos en consola
- Validación de formularios

## 🌟 Próximas Mejoras

- [ ] Base de datos para productos dinámicos
- [ ] Sistema de usuarios y cuentas
- [ ] Integración con pasarelas adicionales
- [ ] Sistema de reseñas y calificaciones
- [ ] API REST para backend
- [ ] Internacionalización (i18n)

## 📄 Licencia

Este proyecto es de código abierto y está disponible bajo la [Licencia MIT](LICENSE).

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! Por favor:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📞 Contacto

**KYRIX STORE**
- Email: support@kyrixstore.com
- GitHub: [@adnanguenfoudi-ux](https://github.com/adnanguenfoudi-ux)
- Sitio Web: [kyrixstore.com](https://adnanguenfoudi-ux.github.io/kyrix.github.io/)

---

⭐ Si te gusta este proyecto, ¡dale una estrella en GitHub!