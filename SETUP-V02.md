# Puesta en marcha v0.2

## Firebase
1. Firebase Console → Authentication → Sign-in method → habilitar Email/Password.
2. En Authentication → Users, agregar manualmente al administrador/taller (no hay registro público).
3. Authentication → Settings → Authorized domains: agregar subbbassgarage-pro.pages.dev.
4. Firestore Database → crear una base de datos en modo producción, si no existe.
5. Firestore Database → Rules: copiar y publicar el contenido exacto de firestore.rules.
6. Abrir la aplicación y entrar a Cuenta online. Entrar, guardar diseño actual en la nube, probar abrir y eliminar. Probar con un segundo usuario que no ve proyectos ajenos.
El SDK web está configurado; no se necesita una clave de servicio. No incluir credenciales administrativas. Auth/Firestore requieren internet. Los proyectos locales y online son guardados explícitos por separado. Cotizaciones permanecen locales; no se sincronizan.

## Funcionalidades y límites
- Prototipo geométrico de caja sellada y bass reflex de puerto ranurado recto.
- Motor de pequeña señal: parámetros de altavoces idénticos y conexión en paralelo, excitación de voltaje de referencia a partir de Re, pérdidas del puerto simplificadas; SPL ideal en semiespacio, no en automóvil real. Filtros de segundo orden, ganancia de cabina aproximada, curvas de excursión, puerto, impedancia, fase y retardo. Verificar parámetros de bobinas y contrastar con WinISD/mediciones. Se probó por ejecución de funciones con 301 muestras finitas sobre dos casos sintéticos, sin validación de precisión externa.
- Vista 3D ortográfica interactiva SVG; no CAD exacto, sin perforaciones ni refuerzos editables.
- Distribución heurística de rectángulos en planchas y exportación CSV/DXF; no optimización global, no código CNC.
- Herramientas nominales de impedancia, consumo, duración teórica de batería.
- Bandpass: cálculo preliminar independiente de cámaras, sin acoplamiento ni planos.
- WDR de texto: reconoce pares clave=valor y aplica solo Fs/Qts. WDR binario, unidades y catálogo personalizado completo pendientes.
- Cotizaciones locales (precio, recargo sobre costo, impuesto editable), cliente asociado e impresión.
- PWA básica y caché de archivos locales: requiere primera carga por HTTPS. El login y los catálogos externos requieren internet.

Pendiente: validar en navegador y Firebase, contrastar simulación con WinISD, geometrías avanzadas completas (invertida, bandpass acoplada, radiador pasivo, horn, línea de transmisión e isobárica), planos con cotas y perforaciones, gestión independiente de clientes, sincronización de cotizaciones, catálogo ampliable y PDF técnico.
