# Configuración de PayPal en KYRIX STORE

## Pasos para obtener tu Client ID de PayPal

### 1. Acceder a PayPal Developer
1. Ve a https://developer.paypal.com
2. Inicia sesión con tu cuenta PayPal (adnanguenfoudi@gmail.com)

### 2. Obtener Client ID
1. En el dashboard, ve a **Apps & Credentials**
2. Asegúrate de estar en el ambiente **Sandbox** primero (para pruebas)
3. Busca la sección **REST API apps**
4. Haz clic en **Create App** si aún no tienes una
5. Copia el **Client ID** de tu aplicación

### 3. Reemplazar en el código
1. Abre el archivo `index.html`
2. Busca esta línea (línea ~625):
   ```html
   <script src="https://www.paypal.com/sdk/js?client-id=YOUR_PAYPAL_CLIENT_ID&currency=USD"></script>
   ```
3. Reemplaza `YOUR_PAYPAL_CLIENT_ID` con tu Client ID real

### 4. Pasar a Producción (cuando estés listo)
- Cuando tu tienda esté lista, cambia `sandbox` a `live` en el SDK
- Ten en cuenta que en producción se cobrará a los clientes realmente

## Ejemplo Final
```html
<script src="https://www.paypal.com/sdk/js?client-id=ABC123XYZ&currency=USD"></script>
```

## Funcionalidades Implementadas

✅ **Sistema de Pago**
- Botón de pago seguro de PayPal
- Cálculo automático del total
- Detalles de cada producto

✅ **Validación**
- El carrito vacío muestra un mensaje
- El botón se actualiza según los items

✅ **Después del Pago**
- Confirmación del pedido
- ID de pedido PayPal guardado
- Carrito se limpia automáticamente
- Información del comprador capturada

## Notas de Seguridad

⚠️ El Client ID es público (está en el frontend), así que es seguro compartirlo
⚠️ Los datos sensibles se procesan en los servidores de PayPal (seguros)
⚠️ Verifica tu cuenta PayPal en Sandbox primero antes de usar en producción

## Pruebas en Sandbox

Para probar sin dinero real:
1. Usa tarjetas de prueba de PayPal
2. Ve a: https://developer.paypal.com/docs/platforms/sandboxes/testing/
3. Usa cuentas de prueba para comprador y vendedor

---

¿Preguntas? Consulta la documentación oficial:
https://developer.paypal.com/docs/checkout/
