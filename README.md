# ForeverTech

**ForeverTech** es una tienda online especializada en productos tecnológicos sin obsolescencia programada. Su objetivo es ofrecer dispositivos electrónicos duraderos, reparables y sostenibles, combinando tecnología moderna con conciencia ambiental.

La aplicación ha sido desarrollada como una plataforma completa e intuitiva tanto para usuarios como para administradores, integrando funcionalidades avanzadas como gestión de R-Coins, panel de administración, compras a través de un carrito, pasarela de pago simulada y más.

---

## 👤 Uso de la aplicación

### Para usuarios
Los usuarios pueden:

- Registrarse o iniciar sesión con su cuenta de Google o correo/contraseña mediante Firebase.
- Navegar por el catálogo de productos electrónicos.
- Añadir productos al carrito y realizar pedidos usando **R-Coins**, una moneda virtual del sistema.
- Comprar paquetes de R-Coins con dinero real mediante una pasarela de pago simulada.
- Consultar su historial de pedidos.
- Gestionar su cuenta personal.

### Para administradores
Los administradores tienen acceso a:

- Gestión completa de usuarios (ver, modificar R-Coins, asignar roles).
- Gestión de productos (crear, editar, eliminar, controlar stock).
- Gestión de pedidos (visualizar todos los pedidos, revocar y reembolsar).
- Gestión de ofertas de R-Coins.
- Interfaz separada para administración con control de accesos.

---

## 🧩 Estructura del proyecto

### Backend (Django)

- **Modelos**: Representan los datos principales como usuarios, productos, pedidos y ofertas.
- **API REST**: Expuesta para que el frontend consuma todas las funcionalidades.
- **Autenticación**: Integración con Firebase para validar usuarios de forma segura.
- **Tareas en segundo plano**: Soporte para tareas asíncronas usando Celery + Redis.
- **Interfaz de administración**: Herramienta para supervisar y gestionar el sistema.

### Frontend (Vue 3 + TypeScript)

- **Vue Router**: Para navegación entre vistas (Login, Productos, Carrito, etc.).
- **Pinia**: Para el manejo global del estado (usuario, carrito, productos).
- **Componentes**: Interfaz modular, responsive, accesible y con diseño adaptado.
- **Views**: Separación clara entre vistas de usuario y administración.
- **Sistema de R-Coins**: Integración directa con el backend para comprar y gastar monedas virtuales.

---

## 🧠 Tecnologías destacadas

- 🔧 **Django** como backend robusto con ORM y administración nativa.
- 🔐 **Firebase Auth** para autenticación segura.
- 🧮 **Vue 3 Composition API** para el frontend moderno y reactivo.
- 🧠 **TypeScript** para desarrollo tipado y seguro.
- 💬 **Pinia** como sistema de gestión de estado.
- 🚀 **Redis + Celery** para tareas en segundo plano.
- 🎨 **Bootstrap 5** para diseño base y responsive.

---

## 🌱 Valores del proyecto

ForeverTech no es solo una tienda, es una declaración contra la cultura del descarte. Aquí, el foco está en:

- Durabilidad real de los productos.
- Rechazo de la obsolescencia programada.
- Compra informada y ética.
- Soporte técnico y postventa real.
- Compromiso con la sostenibilidad social, económica y ambiental.

---

Este proyecto es una solución completa de e-commerce consciente, pensada desde el diseño para ser extensible, mantenible y respetuosa con el entorno y con sus usuarios.

# Conclusión - Un resumen de todo lo usado.

El proyecto **ForeverTech** se ha desarrollado como una tienda online moderna, sostenible e innovadora, cuidando cada uno de los aspectos técnicos, de diseño y de estrategia necesarios para asegurar su funcionalidad, accesibilidad, escalabilidad y éxito comercial. Desde sus primeros pasos, el sistema ha permitido que los usuarios inicien sesión con sus credenciales de forma segura, integrando la autenticación mediante Firebase, lo que asegura un sistema fiable y moderno de gestión de identidades. Además, se han creado diferentes tipos de usuarios, con distintos roles claramente definidos, entre ellos administradores y usuarios estándar, lo cual permite gestionar permisos y vistas específicas en función del tipo de cuenta.

En lo relativo a la seguridad, se ha automatizado la validación de contraseñas gracias al uso del sistema de autenticación de Firebase, el cual impone políticas robustas de seguridad, como la longitud mínima, la complejidad de caracteres y la verificación del correo electrónico. Esta integración garantiza que el sistema cumple con estándares modernos en cuanto a protección de datos y acceso. Asimismo, la gestión de usuarios (altas, bajas y modificaciones) está completamente integrada tanto en el frontend como en el backend, sincronizándose con Firestore para reflejar en tiempo real cualquier cambio en la base de datos.

En el ámbito de la estrategia empresarial, se han desarrollado tanto el **plan de marketing** como el **plan de sostenibilidad** con el máximo detalle. El plan de marketing define con claridad al cliente ideal, el análisis de competencia, las tendencias actuales del mercado y desarrolla una propuesta de valor basada en la durabilidad y sostenibilidad tecnológica. Además, incluye estrategias de promoción concretas mediante SEO, SEM, redes sociales, alianzas con influencers responsables y campañas de fidelización mediante el sistema de R-Coins. Por su parte, el plan de sostenibilidad contempla la viabilidad económica a largo plazo, la sostenibilidad social mediante accesibilidad y ética digital, y la sostenibilidad ambiental a través del uso de hosting verde, un diseño optimizado y la digitalización integral de los procesos.

El diseño del proyecto se ha centrado en ofrecer una experiencia moderna y accesible para todos los usuarios. Para ello, se ha utilizado **Bootstrap** como uno de los frameworks principales de diseño, asegurando una base sólida de estilos y componentes reutilizables. Se ha garantizado la **adaptabilidad** en toda la interfaz, con un diseño **responsive** que permite el uso fluido en ordenadores, tablets y móviles, gracias al uso de técnicas CSS modernas y la integración de Bootstrap Vue. La **accesibilidad** y **usabilidad** también han sido prioridades, aplicando contrastes adecuados, estructura semántica y soporte de navegación mediante teclado, todo ello con una interfaz intuitiva y amigable.

Desde el punto de vista del backend, se ha utilizado **Django** como motor principal. Se han creado y gestionado modelos utilizando el ORM incorporado, facilitando las operaciones CRUD y asegurando la integridad relacional de la base de datos. Además, el proyecto cuenta con una **interfaz administrativa personalizada**, donde los administradores pueden gestionar usuarios, productos, pedidos y ofertas de R-Coins. También se ha implementado una **API RESTful**, que permite la interacción eficiente entre frontend y backend, con endpoints protegidos por autenticación y estructurados de forma clara y escalable. Para tareas asincrónicas, como el envío de correos electrónicos o la gestión de eventos demorados, se han utilizado **tareas desacopladas** con Celery y Redis como sistema de colas de mensajes.

En cuanto al frontend, se ha empleado **Vue 3** en su máxima expresión, conectado al backend de Django mediante llamadas API. El proyecto hace uso del **Composition API**, estructurado mediante **Single File Components (SFC)** para una organización clara y modular del código. Se ha utilizado **TypeScript** en combinación con **ESLint**, lo que permite escribir código robusto, tipado y limpio. Además, se usan **directivas personalizadas**, así como **props y emits** para la comunicación entre componentes, junto con **Pinia** como sistema de gestión del estado global. También se ha implementado el uso de `localStorage` para guardar datos como tokens o información persistente del carrito, y `sessionStorage` cuando es necesario mantener datos solo durante la sesión activa.

El proyecto integra un **Router** con rutas protegidas y redireccionamientos inteligentes en función del rol del usuario. Se han utilizado **composables** para abstraer lógica reutilizable (como funciones de carrito o autenticación), y también se ha hecho uso de **slots** para componentes reutilizables que requieren contenido dinámico. Todo el frontend está fuertemente tipado mediante **interfaces**, lo que mejora la robustez del sistema. Finalmente, se han desarrollado **tests unitarios** para componentes críticos del frontend, asegurando su correcto funcionamiento con pruebas automatizadas que validan estados, interacciones y salidas esperadas.

En definitiva, **ForeverTech** es un proyecto integral, cuidadosamente estructurado y documentado, que cumple con todos los requisitos técnicos y estratégicos, y que ha sido desarrollado con un alto nivel de calidad, innovación y compromiso con la sostenibilidad.


## ✅ PLAN DE MARKETING

### **1.1 Análisis de mercado**

* **Cliente ideal (buyer persona)**:
  Adultos de 25 a 45 años con conciencia ambiental y tecnológica. Valoran la durabilidad, la ética de producción y el soporte a largo plazo. Profesionales del sector IT, estudiantes de ingeniería, diseñadores, y consumidores exigentes que rechazan la obsolescencia programada.

* **Competencia**:
  Competimos con grandes marketplaces como Amazon o PcComponentes, aunque nos diferenciamos claramente en valores (durabilidad, sostenibilidad). También con pequeñas tiendas especializadas que priorizan soporte técnico, pero sin nuestra propuesta de valor sostenible.

* **Tendencias del mercado**:
  Aumento del interés por productos éticos y sostenibles. Los consumidores cada vez investigan más antes de comprar. Crece la demanda de productos reparables, con soporte postventa prolongado y garantías extendidas. Las políticas europeas están favoreciendo el derecho a la reparación.

---

### **1.2 Propuesta de valor**

ForeverTech ofrece **productos electrónicos sin obsolescencia programada**, seleccionados por su **durabilidad, reparabilidad y soporte técnico real a largo plazo**.
Además, nuestro sistema de compra con **R-Coins** premia la fidelidad, facilita promociones personalizadas y fomenta el ahorro en próximas compras.

> 🔸 *"ForeverTech: Tecnología que no caduca."*

---

### **1.3 Estrategias de promoción y publicidad**

* **Marketing digital**:

  * SEO: Contenido optimizado en blog sobre sostenibilidad tecnológica, comparativas de productos duraderos.
  * SEM: Campañas en Google Ads y redes sociales con palabras clave como “productos sin obsolescencia programada”.

* **Contenidos y redes sociales**:

  * Instagram y TikTok: Reels de “productos que duran 10 años”, desmontajes de hardware reparable, consejos para alargar la vida útil de gadgets.
  * YouTube: Mini-documentales y comparativas sobre el impacto ambiental de la tecnología desechable.
  * Blog técnico y de opinión en la web.

* **Alianzas**:

  * Colaboración con ONGs tecnológicas y asociaciones de consumidores.
  * Afiliación con influencers y youtubers tech responsables.

---

### **1.4 Estrategia de ventas y precios**

* **Modelo de precios**:

  * Precios competitivos, ajustados al valor a largo plazo del producto (TCO: coste total de propiedad).
  * Sistema de recompensas con R-Coins por cada compra.
  * Descuentos escalonados por fidelidad o volumen.

* **Técnicas de venta**:

  * **Cross-selling**: Sugerencias de accesorios duraderos compatibles al añadir un producto al carrito.
  * **Upselling**: Recomendaciones de versiones más potentes con garantía extendida sin obsolescencia.
  * **Bundles sostenibles**: Packs de productos duraderos con instalación o formación técnica.

---

## **1.5 Medición y KPIs (Indicadores clave de rendimiento)**

Para que la estrategia de marketing sea realmente efectiva, necesitamos evaluar de forma **continua y objetiva** su impacto. Para ello, definimos una serie de KPIs (Key Performance Indicators) que nos permitirán tomar decisiones basadas en datos reales, detectar errores a tiempo y optimizar nuestras campañas y procesos de venta.

### **Conversión**

* **Definición**: Porcentaje de visitantes que realizan una compra en la tienda online.
* **Cálculo**:

  Tasa de conversión = Nº de pedidos / Nº de visitas x 100

* **Objetivo inicial**: 2% (es decir, que de cada 100 personas que visitan la tienda, al menos 2 compren algo).
* **Uso**: Permite medir la eficacia del sitio web, la confianza que genera y la calidad del tráfico que atraemos. Si es baja, revisamos el proceso de compra, la experiencia de usuario o las campañas de adquisición.

---

### **Retención de clientes**

* **Definición**: Porcentaje de clientes que vuelven a comprar en un periodo determinado.
* **Objetivo a 6 meses**: 25% (1 de cada 4 clientes vuelve a comprar).
* **Importancia**: Un cliente que vuelve es más rentable a largo plazo. La retención también indica satisfacción con el producto y la experiencia postventa.
* **Medición**: Seguimiento de cuentas de usuario, historial de pedidos y uso de R-Coins.

---

### **Ticket medio (valor medio del pedido)**

* **Definición**: Promedio de gasto por pedido, medido en euros y en R-Coins.
* **Cálculo**:

  Ticket medio = Ingresos totales / Nº total de pedidos

* **Importancia**: Nos ayuda a diseñar estrategias de upselling y bundles más efectivos. Un ticket medio bajo puede indicar falta de interés en productos complementarios o poco incentivo en las promociones.

---

### **ROI de campañas de marketing**

* **Definición**: Retorno sobre la inversión en publicidad (Google Ads, redes sociales, influencers...).
* **Cálculo**:

  ROI = ((Ganancia generada por la campaña - Coste de la campaña) / Coste de la campaña) x 100

* **Ejemplo**: Si invertimos 200 € en una campaña y generamos 800 € en ventas atribuibles, el ROI es del 300%.
* **Uso**: Detectamos qué campañas funcionan mejor, qué canales son más rentables y dónde optimizar el presupuesto.

---

### **Engagement en redes sociales**

* **Definición**: Grado de interacción del público con nuestro contenido (likes, shares, comentarios, clics).
* **Métricas específicas**:

  * Tasa de interacción (por post y por red).
  * Crecimiento de seguidores.
  * Tiempo de visualización en vídeos.
* **Plataformas clave**: Instagram, TikTok, YouTube.
* **Uso**: El engagement indica la calidad del contenido y el interés real de la audiencia. A mayor interacción, más alcance orgánico y mayor fidelización de marca.

---

### **Satisfacción del cliente (NPS y encuestas post-compra)**

* **Net Promoter Score (NPS)**:

  * Pregunta directa: “¿Recomendarías ForeverTech a un amigo o familiar?”
  * Escala de 0 a 10.

    * Promotores (9–10), Pasivos (7–8), Detractores (0–6).
  * Cálculo:

    NPS = %Promotores − %Detractores

* **Encuestas adicionales**: Valoración del proceso de compra, envío, atención al cliente, calidad del producto.
* **Uso**: Estas métricas reflejan directamente la experiencia del cliente y permiten detectar problemas antes de que afecten la reputación o las ventas.

---

### **Otros indicadores adicionales**

* **Tasa de abandono del carrito**: Si muchos usuarios añaden productos pero no finalizan la compra, hay que revisar el proceso de pago o añadir incentivos.
* **Coste de adquisición por cliente (CAC)**: Cuánto invertimos en conseguir un nuevo cliente.
* **Tiempo medio en el sitio web**: Cuanto más tiempo pasen, más interés existe. Un descenso puede indicar problemas de navegación o velocidad de carga.

---

### 📊 Herramientas para el seguimiento

* **Google Analytics 4**: Para métricas de tráfico, conversión y comportamiento en la tienda.
* **Google Search Console**: Para SEO y rendimiento en búsquedas.
* **Meta Business Suite / TikTok Analytics / YouTube Studio**: Para redes sociales.
* **Plataformas de email marketing**: (como Mailchimp o Brevo) para medir tasas de apertura y clics en campañas.
* **Herramientas internas del backend**: para R-Coins, ticket medio, frecuencia de compra y retención.


## ✅ PLAN DE SOSTENIBILIDAD

### **2.1 Sostenibilidad económica**

* **Modelo rentable y diversificado**:

  * Ingresos por ventas directas y por packs promocionales.
  * Posibilidad de servicios adicionales a largo plazo (formación, soporte, kits de reparación).

* **Control de costes**:

  * Inventario ajustado a demanda gracias a análisis de comportamiento de compra.
  * Plataforma desarrollada internamente, evitando fees de terceros.

* **Uso de R-Coins**:

  * Fomenta la fidelización y reduce costes en adquisición de nuevos clientes.

---

### **2.2 Sostenibilidad social**

* **Accesibilidad**:

  * Plataforma totalmente responsive y con diseño accesible (colores contrastados, navegación por teclado, textos alternativos).
  * Política de precios justos y posibilidad de pago con saldo virtual acumulado (R-Coins).

* **Ética**:

  * Productos seleccionados con criterios éticos (fabricantes comprometidos con la transparencia).
  * Rechazo a modelos de consumo rápido o de baja calidad.

* **Acciones para la comunidad**:

  * Programa de formación gratuita online: “Repara tu tecnología”.
  * Colaboración con colectivos que luchan contra la brecha digital (donaciones de excedente a asociaciones).

---

### **2.3 Sostenibilidad ambiental**

* **Hosting verde**:

  * La web estará alojada en un proveedor que utiliza energías 100% renovables (como GreenGeeks o Infomaniak).

* **Diseño optimizado**:

  * Carga eficiente, imágenes comprimidas, lazy loading y frontend desacoplado (Vue 3).
  * Menor consumo de datos = menor huella de carbono digital.

* **Digitalización de procesos**:

  * Gestión 100% digital de pedidos, facturación y soporte.
  * Evitamos documentación en papel, albaranes físicos o tickets impresos.
  * Preferencia por productos que incluyen manuales digitales y empaque reciclado.
