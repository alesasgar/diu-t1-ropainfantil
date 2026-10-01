# Documentación de la interfaz — RainbowKid

## 1. Justificación del diseño

### 1.1 Importancia del diseño centrado en el usuario
En la app RainbowKid el diseño centrado en el usuario es fundamental ya que las decisiones de compra de ropa infantil se ven condicionadas por la falta de tiempo, el uso del móvil con una sola mano y la duda sobre las tallas. Al centrar la interfaz en las necesidades reales de los padres y familiares se reduce la complicación del uso de la app, y se minimizan los por errores a la hora de comprar.

### 1.2 Objetivos y metas del proyecto
1. **Reducir el tiempo de compra:** Conseguir que un usuario registrado pueda hacer una compra de un producto en menos de **2 minutos**.
2. **Disminuir las devoluciones por talla:** Lograr que al menos el **80%** de los compradores mire la guía de tallas antes del pago interactuando con el boton de la compra.
3. **Navegación a "Una Mano" y Compra Rápida:** Hacer que el **90%** de usuarios de la app le parezca sencillo buscar y comprar los productos mientras hacen alguna tarea.

### 1.3 Beneficios esperados
* **Para el usuario:** Una experiencia rápida, clara e intuitiva que hace que el usuario pueda encontrar el producto adecuado por edad, seleccionar la talla correcta y pagar de forma facil con una mano.
* **Para el negocio:** Incremento de las ventas en el móvil, hacer que el cliente vualva a comprar mediante un perfil y añadir descuentos por hacer compras y vuelva a comprar.

## 2. Investigación y análisis de usuarios

### 2.1 Datos demográficos y segmentación
* **Publico principal:** Madres y padres de entre 30 y 45 años, con un estilo de vida activo, que sepan hacer compras online pero con compras facilitadas para hacerlas mas rapida.
* **Publico secundario:** Abuelos y familiares (30-70 años) que quieren regalar ropa para ocasiones especiales o cumpleaños y necesitan una guia clara en la eleccion de productos segun la edad del niño.

### 2.2 Personas

#### Persona 1: Maria Juana
* **Edad:** 34 años.
* **Contexto:** Trabaja y tiene dos hijos de 1 y 4 años. Compra normalmente en el transporte publico.
* **Objetivos:** Comprar ropa duradera de forma rapida y sin complicaciones de navegacion.
* **Frustraciones:** Formularios de compra eternos, menus dificiles de entender y botones pequeños difíciles de pulsar con el pulgar.

#### Persona 2: Killian Mbappe
* **Edad:** 64 años.
* **Contexto:** Quiere hacerle un regalo a su nieta de 3 años, pero no sabe que comprar por que desconoce la talla.
* **Objetivos:** Encontrar facilmente productos segun la edad y saber que ha aceptado con la talla.
* **Frustraciones:** Tablas de tallas que no entiende con medidas en centimetros complejas de entender y procesos de pago que no son claros.

### 2.3 Análisis de la competencia

| App Competidora | Qué hacen bien | Qué hacen mal | Qué nos llevamos (Aprendizaje) |
| **Mayoral** | Buena categorización por rangos de edad e imágenes de alta calidad. | Proceso de Checkout sobrecargado de pasos y texto pequeño. | Adoptar la estructura limpia de categorías e integrar un Checkout simplificado en un solo flujo. |
| **Zara** | Diseño minimalista, visual y fluido con buenas transiciones. | Filtros escondidos y tipografía con poco contraste o legibilidad. | Mantener un diseño atractivo respetando los contrastes de accesibilidad WCAG AA de Material Design 3. |
| **Vertbaudet** | Excelente guía de tallas e indicaciones según altura/meses del bebé. | Interfaz sobrecargada de promociones que distraen en el carrito. | Crear una guia de tallas clara desplegable mediante un Bottom Sheet sin saturar la pantalla con ofertas. |

### 2.4 Insights y hallazgos clave
1. **Insight 1 Dudas con las tallas:** Los usuarios dudan sobre qué talla elegir según los meses o la altura.
   * *Decisión de diseño:* Implementar un botón destacado «Guía de tallas» en la ficha de producto que abre un una pestaña con referencias a las edades.
2. **Insight 2 Uso en movilidad con una mano:** Las compras se realizan en momentos de prisa usando únicamente el pulgar.
   * *Decisión de diseño:* Situar los destinos principales en la barra de navegación inferior y asegurar que todos los botones principales tengan un área táctil amplia.
3. **Insight 3 Eliminación accidental de productos:** Borrar por error un elemento del carrito causa frustración y abandono.
   * *Decisión de diseño:* Añadir un botón de confirmación para eliminar el producto.
4. **Insight 4 Búsqueda de regalo:** Compradores como abuelos o amigos buscan por rangos de edad especificos.
   * *Decisión de diseño:* Hacer un filtro por categorias para los productos Bebé 0-24 m, Niña, Niño.