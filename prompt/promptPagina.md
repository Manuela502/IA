# NUTRIBUDGET — PROMPT MAESTRO DE DISEÑO Y DESARROLLO

Actúa como un equipo multidisciplinario conformado por:

- Product Owner especializado en productos digitales.
- Arquitecto de software senior.
- Ingeniero de software Full Stack.
- Diseñador UX/UI especializado en productos SaaS y FoodTech.
- Especialista en diseño de bases de datos.
- Analista de requisitos.
- Ingeniero QA.

Tu objetivo es diseñar y construir **NutriBudget**, una aplicación web funcional, moderna, intuitiva y escalable, basada en el documento de especificación de requisitos de software (SRS) y su posterior auditoría técnica.

No quiero una página web genérica ni únicamente una landing page. Quiero una aplicación que represente correctamente el producto, sus funcionalidades, sus reglas de negocio y la experiencia de usuario completa.

---

# 1. DOCUMENTACIÓN DE REFERENCIA

Te proporcionaré dos documentos:

1. **NutriBudget SRS v1.0 — noviembre de 2026:** contiene la definición del producto, problema, objetivos, usuarios, requisitos funcionales y no funcionales, historias de usuario, arquitectura, modelo de datos, reglas de negocio, MVP y pruebas.
2. **Análisis del SRS de NutriBudget:** contiene una auditoría técnica que identifica inconsistencias, riesgos, propuestas de corrección, mejoras del modelo de datos y recomendaciones de arquitectura.

Debes leer ambos documentos completos antes de comenzar.

El SRS establece la definición original del producto. El análisis técnico complementa esa definición y propone correcciones.

Debes respetar los requisitos y las recomendaciones técnicas, pero distinguir entre:
- Requisitos ya definidos.
- Correcciones propuestas por la auditoría.
- Decisiones de negocio pendientes de aprobación.
- Mejoras que corresponden a futuras versiones.

No inventes funcionalidades ni conviertas automáticamente propuestas pendientes en decisiones definitivas.

# 2. VISIÓN DEL PRODUCTO

## ¿Qué es NutriBudget?

NutriBudget es una aplicación web que ayuda a personas y hogares a organizar su alimentación de acuerdo con su presupuesto, los ingredientes que tienen disponibles y sus preferencias alimentarias.

Su propósito es facilitar la planificación de comidas, optimizar las compras y reducir el desperdicio de alimentos.

**Propuesta de valor:**

"Alimentación inteligente, saludable y económica".

NutriBudget conecta cuatro elementos fundamentales:

1. Presupuesto disponible.
2. Inventario de alimentos.
3. Planificación de menús y recetas.
4. Lista de compras optimizada.

La aplicación debe responder una pregunta central:

**¿Cómo puedo organizar las comidas de mi semana, aprovechar los ingredientes que ya tengo y comprar únicamente lo necesario sin superar mi presupuesto?**

## Problemas que busca solucionar

- Las personas no saben cómo organizar sus comidas durante la semana.
- Es difícil determinar cuánto dinero se necesita para alimentarse durante un periodo.
- Se compran ingredientes que ya existen en casa.
- Se desperdician alimentos por falta de planificación.
- Muchas recetas no se ajustan al presupuesto disponible.
- No existe una conexión clara entre recetas, inventario y compras.
- Es complicado controlar cuánto dinero se gasta realmente en alimentación.

## Público objetivo

La aplicación está orientada a:

- Estudiantes.
- Personas que viven solas.
- Jóvenes independientes.
- Familias y hogares.
- Personas que buscan organizar sus gastos de alimentación.
- Personas interesadas en reducir el desperdicio de alimentos.

El mercado inicial es Colombia y la moneda de referencia es el peso colombiano (COP).

# 3. OBJETIVO DEL PROTOTIPO

Construye un prototipo web de alta fidelidad que permita recorrer y probar los principales flujos de NutriBudget.

Debe incluir:
- Interfaz visual completa.
- Navegación entre módulos.
- Formularios funcionales.
- Información de ejemplo realista.
- Interacciones que produzcan resultados visibles.
- Estados de carga, vacío, error y confirmación.
- Datos de demostración.
- Diseño responsive.
- Experiencia coherente entre todos los módulos.

No te limites a crear pantallas estáticas.

Por ahora, utiliza datos simulados y servicios desacoplados para representar las operaciones. No conectes una base de datos externa ni implementes una autenticación de producción sin aprobación.

Los datos de demostración deben permitir explorar las funcionalidades y comprobar los flujos del producto.

# 4. ARQUITECTURA Y TECNOLOGÍA

## Arquitectura objetivo del producto definitivo

La arquitectura establecida en el SRS es:

**Frontend**
- Angular.
- TypeScript.
- HTML5.
- CSS3.

**Backend**
- Java.
- Spring Boot.
- Spring Security.
- Spring Data JPA.
- Hibernate.
- API REST.

**Base de datos**
- PostgreSQL.

**Arquitectura**
- Monolito modular.
- Separación de responsabilidades.
- Comunicación mediante API REST.

## Consideración para Lovable

Reconoce las limitaciones del entorno de Lovable y utiliza el stack nativo que la plataforma proporcione.

No intentes presentar React o TanStack Start como si fueran Angular.

No reemplaces ni modifiques la arquitectura objetivo del producto definitivo.

Organiza el prototipo por módulos, componentes reutilizables, tipos de datos y servicios independientes, de manera que la lógica de negocio pueda trasladarse posteriormente a Angular y el backend pueda implementarse en Java con Spring Boot.

Separa claramente:
- Presentación.
- Componentes.
- Modelos y tipos.
- Servicios de datos.
- Reglas de negocio.
- Estado de la aplicación.

No utilices Supabase ni otro backend administrado sin autorización.

No implementes funcionalidades que dependan de servicios externos que no estén configurados.

# 5. IDENTIDAD VISUAL Y DESIGN SYSTEM

Quiero una interfaz que transmita:

- Alimentación.
- Bienestar.
- Organización.
- Ahorro.
- Confianza.
- Sencillez.
- Tecnología.

Debe sentirse como un producto FoodTech moderno, no como una plantilla administrativa genérica.

## Paleta de colores oficial

Utiliza los colores definidos en el SRS:

| Color | Hexadecimal | Uso |
|---|---|---|
| Verde principal | #2E7D5B | Acciones principales y marca |
| Verde claro | #E7F3EC | Fondos suaves y estados positivos |
| Crema | #FAF7F0 | Fondo general |
| Amarillo | #F2C66D | Acentos y alertas suaves |
| Gris oscuro | #303A36 | Textos principales |
| Blanco | #FFFFFF | Superficies y tarjetas |

## Tipografías

- Manrope: títulos y encabezados.
- Inter: textos, formularios y elementos de interfaz.

## Dirección visual

Diseña una interfaz:
- Minimalista.
- Elegante.
- Moderna.
- Limpia.
- Amigable.
- Profesional.
- Fácil de navegar.

Utiliza espacios generosos, jerarquía tipográfica clara, tarjetas bien organizadas, bordes sutiles y radios moderados.

Evita:
- Diseños genéricos de dashboards.
- Gradientes excesivos.
- Sombras exageradas.
- Colores saturados.
- Tarjetas innecesarias.
- Iconografía inconsistente.
- Demasiados elementos en una misma pantalla.
- Apariencia de plantilla predeterminada de un generador de aplicaciones.

Crea un sistema visual consistente con:
- Colores semánticos.
- Escala tipográfica.
- Espaciado.
- Radios.
- Elevaciones.
- Botones.
- Campos de formulario.
- Tarjetas.
- Modales.
- Alertas.
- Etiquetas de estado.
- Navegación.

Utiliza tokens de diseño reutilizables. Evita Bootstrap y no dependas de estilos genéricos que impidan personalizar la interfaz.

# 6. ESTRUCTURA GENERAL DE LA APLICACIÓN

La aplicación debe tener dos experiencias principales:

## A. Sitio público

Ruta inicial `/`

Debe presentar NutriBudget a usuarios nuevos.

Incluye:

- Header con logotipo y navegación.
- Hero principal.
- Propuesta de valor.
- Explicación de cómo funciona.
- Beneficios principales.
- Presentación de funcionalidades.
- Sección de ahorro y aprovechamiento de alimentos.
- Llamado a la acción para registrarse.
- Footer.

El hero debe comunicar claramente que NutriBudget permite planificar la alimentación según el presupuesto y los ingredientes disponibles.

Evita titulares comerciales genéricos.

## B. Aplicación privada

Después del acceso, el usuario debe ingresar a un espacio de trabajo organizado.

Incluye:
- Sidebar de navegación en escritorio.
- Header superior.
- Nombre y avatar del usuario.
- Accesos rápidos.
- Contenido principal.
- Navegación responsive en dispositivos móviles.

La navegación debe incluir:

1. Dashboard.
2. Mi presupuesto.
3. Mi inventario.
4. Recetas.
5. Planificador semanal.
6. Lista de compras.
7. Seguimiento de gastos.
8. Historial.
9. Perfil y preferencias.

Para el rol ADMIN, incorpora una navegación administrativa independiente.

# 7. MÓDULOS Y FUNCIONALIDADES

## MÓDULO 1. AUTENTICACIÓN Y USUARIOS

Requisitos relacionados: RF-01, RF-02 y RF-20.

Construye las pantallas de:

- Registro.
- Inicio de sesión.
- Cierre de sesión.
- Perfil del usuario.
- Eliminación de cuenta.

### Registro

Campos:
- Nombre.
- Correo electrónico.
- Contraseña.
- Confirmación de contraseña.
- Aceptación de términos y condiciones.
- Aceptación del tratamiento de datos personales.

Incluye validaciones y mensajes de error comprensibles.

El registro debe contemplar aceptación de términos y almacenar conceptualmente la fecha de aceptación (`terms_accepted_at`).

La recuperación de contraseña está pendiente de aprobación y no debe implementarse como una funcionalidad real.

## MÓDULO 2. ONBOARDING Y PERFIL ALIMENTARIO

Requisitos relacionados: RF-03 y RF-05.

Después del registro, presenta un proceso de configuración dividido en tres pasos:

**Paso 1. Perfil y hogar**
- Nombre del usuario.
- Número de integrantes.
- Preferencias alimentarias.
- Restricciones alimentarias.
- Alergias e intolerancias.
- Ingredientes excluidos.
- Comidas que desea planificar.

**Paso 2. Presupuesto**
- Valor disponible.
- Periodo semanal.
- Fecha de inicio.
- Fecha de finalización.

**Paso 3. Inventario**
- Agregar ingredientes disponibles.
- Registrar cantidades.
- Seleccionar unidades.
- Registrar fecha de consumo preferente.
- Opción para omitir este paso.

El inventario debe ser opcional. El usuario debe poder generar un menú aunque todavía no tenga ingredientes registrados.

Distingue correctamente:
- Preferencias alimentarias.
- Restricciones alimentarias.
- Alergias e intolerancias.
- Exclusiones voluntarias.

No representes estas categorías como si fueran equivalentes.

## MÓDULO 3. DASHBOARD

Este es el centro de control del usuario.

Debe presentar información resumida y útil.

Incluye:

### Resumen del presupuesto
- Presupuesto semanal.
- Gastos registrados.
- Saldo disponible.
- Porcentaje utilizado.

### Resumen de alimentación
- Próxima comida.
- Menú del día.
- Comidas planificadas.
- Comidas completadas.

### Inventario
- Ingredientes disponibles.
- Ingredientes próximos a su fecha de consumo preferente.
- Ingredientes que requieren reposición.

### Compras
- Costo estimado de compras pendientes.
- Cantidad de productos por comprar.
- Acceso directo a la lista de compras.

### Indicadores visuales

Utiliza gráficas sencillas únicamente cuando aporten valor.

Incluye mensajes útiles como:

- "Estás dentro de tu presupuesto".
- "Tienes ingredientes que puedes aprovechar".
- "Tu próxima comida está programada para hoy".
- "Tu lista de compras tiene 5 ingredientes pendientes".

El dashboard debe tener estados vacíos cuando el usuario todavía no haya configurado su información.

La incorporación del dashboard como requisito independiente corresponde a una propuesta del análisis técnico (RF-21), pendiente de formalización en el SRS.

## MÓDULO 4. PRESUPUESTO

Requisito relacionado: RF-04.

Permite:

- Crear presupuesto semanal.
- Consultar presupuesto.
- Modificar presupuesto.
- Consultar gastos acumulados.
- Visualizar saldo.
- Comparar costos estimados y reales.

El valor monetario debe mostrarse en pesos colombianos.

Utiliza formato:

`$ 150.000 COP`

Evita inconsistencias en los cálculos.

Distingue:
- Costo total estimado de las recetas.
- Costo estimado de los ingredientes que faltan por comprar.
- Dinero realmente gastado.

La auditoría recomienda medir la viabilidad del presupuesto utilizando `estimated_purchase_cost`, es decir, el costo de lo que realmente falta comprar.

Esta decisión todavía debe aprobarse.

No confundas el costo completo de una receta con el dinero que necesita desembolsar el usuario.

## MÓDULO 5. INVENTARIO

Requisitos relacionados: RF-06 y RF-07.

Permite administrar los ingredientes disponibles en casa.

Cada registro debe incluir:

- Ingrediente.
- Cantidad.
- Unidad.
- Fecha de consumo preferente.
- Fecha de registro.

El diseño debe permitir múltiples lotes del mismo ingrediente con diferentes fechas de consumo preferente.

Organiza la información mediante:
- Ingredientes disponibles.
- Próximos a consumirse.
- Inventario agotado o insuficiente.

Incluye:
- Agregar ingrediente.
- Editar cantidad.
- Eliminar ingrediente.
- Buscar ingrediente.
- Filtrar por categoría.
- Ordenar por fecha de consumo preferente.

El sistema debe contemplar unidades base:
- Gramos (g).
- Mililitros (ml).
- Unidades (unit).

Las cantidades deben manejarse internamente en la unidad base del ingrediente.

La interfaz puede mostrar unidades de presentación como kg, litros o unidades comerciales mediante conversiones consistentes.

La lógica de aprovechamiento del inventario debe priorizar los ingredientes cuya fecha de consumo preferente esté más próxima.

## MÓDULO 6. RECETARIO

Requisito relacionado: RF-08.

Construye un catálogo de recetas que pueda explorarse mediante tarjetas visuales.

Cada receta debe presentar:

- Fotografía.
- Nombre.
- Descripción.
- Tiempo de preparación.
- Tipo de comida.
- Número de porciones.
- Ingredientes.
- Cantidades.
- Preparación.
- Grupo de alimentos.
- Costo estimado.
- Etiquetas alimentarias.

Incluye filtros por:
- Desayuno.
- Almuerzo.
- Cena.
- Tiempo de preparación.
- Ingredientes.
- Categorías.
- Preferencias alimentarias.
- Costo aproximado.

Crea una página de detalle de receta.

Utiliza recetas reconocibles y apropiadas para el contexto colombiano.

Para la demostración incluye recetas como:
- Arepa con huevo.
- Avena casera.
- Arroz con pollo.
- Lentejas guisadas.
- Sudado de pollo.
- Ensalada de garbanzos.
- Tortilla de vegetales.
- Pasta con verduras.
- Fríjoles.
- Sopa de verduras.
- Arroz con huevo.
- Crema de ahuyama.

Los precios utilizados en la demostración deben estar identificados como estimaciones de ejemplo, no como precios reales verificados de supermercados.

No inventes información nutricional médica.

## MÓDULO 7. PLANIFICADOR Y GENERADOR DE MENÚS

Este es el módulo más importante de NutriBudget.

Requisitos relacionados: RF-09, RF-10, RF-11 y RF-12.

Debe permitir generar un menú semanal según:

- Presupuesto.
- Número de integrantes.
- Inventario disponible.
- Preferencias alimentarias.
- Alergias e intolerancias.
- Ingredientes excluidos.
- Comidas seleccionadas.
- Recetas existentes.
- Costos estimados.

### Configuración del menú

El usuario debe poder seleccionar:

- Semana que desea planificar.
- Número de personas.
- Presupuesto.
- Comidas que desea incluir.
- Preferencias.
- Restricciones.
- Ingredientes que desea aprovechar.

Las comidas propuestas inicialmente son:
- Desayuno.
- Almuerzo.
- Cena.

La configuración final de comidas queda sujeta a confirmación.

### Resultado

Presenta un calendario semanal organizado por días y comidas.

Cada elemento debe mostrar:
- Nombre de la receta.
- Imagen.
- Tiempo de preparación.
- Porciones.
- Costo estimado.
- Disponibilidad de ingredientes.

El usuario debe poder:

- Consultar el detalle.
- Cambiar una receta por otra.
- Modificar una preparación.
- Regenerar el menú.
- Consultar el presupuesto estimado.
- Ver los ingredientes disponibles y faltantes.

### Resumen económico

Presenta claramente:

1. Costo total estimado de las recetas.
2. Valor estimado de ingredientes que ya existen en inventario.
3. Costo estimado de compra de ingredientes faltantes.
4. Presupuesto disponible.
5. Saldo estimado.

### Reglas esenciales del generador

La auditoría detectó errores importantes que deben evitarse:

- No descontar inventario varias veces cuando un ingrediente aparece en diferentes recetas.
- Primero sumar las necesidades totales del menú por ingrediente.
- Después descontar el inventario disponible una sola vez.
- Comparar cantidades con unidades compatibles.
- No seleccionar recetas incompatibles con alergias o restricciones.
- Priorizar ingredientes próximos a su fecha de consumo preferente.
- Considerar la variedad de recetas.
- Considerar grupos de alimentos.
- Evitar superar el presupuesto disponible.

El algoritmo propuesto debe usar reglas y puntuaciones, no inteligencia artificial ni aprendizaje automático obligatorio.

Para el prototipo, simula de manera coherente la generación de menús con datos de ejemplo.

No implementes una generación aleatoria sin respetar las restricciones.

### Sustituciones

Hay una diferencia entre:
- Cambiar una receta del menú por otra.
- Sustituir un ingrediente por otro equivalente.

El cambio de receta forma parte del MVP propuesto.

La sustitución de ingredientes requiere una tabla específica de equivalencias y se recomienda diferirla hasta que el equipo confirme su inclusión.

No mezcles estas dos funcionalidades.

## MÓDULO 8. LISTA DE COMPRAS

Requisito relacionado: RF-13.

La lista debe generarse a partir del menú semanal.

Debe incluir:
- Nombre del ingrediente.
- Cantidad necesaria.
- Unidad.
- Cantidad disponible en inventario.
- Cantidad que falta comprar.
- Precio estimado.
- Subtotal.

Agrupa ingredientes repetidos en diferentes recetas.

No repitas un ingrediente por cada preparación.

Incluye:
- Casillas para marcar productos.
- Filtros por categoría.
- Total estimado.
- Productos pendientes.
- Productos marcados.
- Estado de la lista.

La lista de compras debe estar asociada de forma única a un menú semanal.

La opción de marcar un producto como comprado es diferente de registrar formalmente una compra.

## MÓDULO 9. COMPRAS Y SEGUIMIENTO DE GASTOS

Requisitos relacionados: RF-14, RF-15 y RF-16.

Permite registrar compras reales.

Cada compra debe incluir:
- Fecha.
- Productos.
- Cantidades.
- Valor real de cada línea.
- Total de la compra.
- Presupuesto asociado.
- Lista de compras relacionada, cuando exista.

Distingue el precio estimado del precio real.

La información real debe permitir comparar:

- Presupuesto inicial.
- Costo estimado.
- Costo real.
- Diferencia.
- Saldo disponible.

Considera que los ingredientes pueden comprarse en paquetes o cantidades comerciales superiores a las necesarias para una receta.

El costo registrado debe corresponder al valor real pagado (`line_total`), no a un precio unitario artificialmente redondeado.

El sobrante de una compra puede incorporarse al inventario.

Una compra puede completar parcialmente una lista.

## MÓDULO 10. HISTORIAL

Permite consultar:

- Menús anteriores.
- Presupuestos.
- Compras.
- Gastos.
- Recetas utilizadas.
- Evolución del presupuesto.
- Historial de planificación.

Debe existir consistencia entre los datos históricos y los datos actuales.

Los costos asociados a planes anteriores deben conservarse aunque cambien los precios del catálogo.

## MÓDULO 11. ADMINISTRACIÓN

Roles del sistema:
- USER.
- ADMIN.

El administrador debe disponer de un espacio separado.

Incluye pantallas para:

### Gestión de recetas
- Crear recetas.
- Editar recetas.
- Desactivar recetas.
- Administrar ingredientes.
- Administrar porciones.
- Administrar tiempos.
- Clasificar tipos de comida.
- Asociar grupos alimentarios.

### Gestión de ingredientes
- Crear ingredientes.
- Editar ingredientes.
- Administrar unidades base.
- Administrar categorías.
- Clasificar grupos de alimentos.
- Definir conflictos con etiquetas alimentarias.

### Gestión de precios
- Registrar precios.
- Actualizar precios.
- Consultar fuente.
- Consultar fecha de actualización.
- Identificar precios desactualizados.

Los usuarios normales no deben acceder a las herramientas administrativas.

La fuente definitiva de precios queda pendiente de decisión.

# 8. REGLAS DE NEGOCIO IMPORTANTES

Debes considerar las siguientes reglas al diseñar las interacciones:

1. El presupuesto debe tener un valor positivo.
2. No deben existir presupuestos semanales solapados para un mismo usuario.
3. El plan debe estar dentro del periodo de su presupuesto.
4. El número de personas debe ser mayor que cero.
5. Las recetas deben tener cantidades y porciones válidas.
6. Los ingredientes deben tener unidades consistentes.
7. Las alergias y restricciones deben excluir recetas incompatibles.
8. El inventario debe permitir lotes diferentes del mismo ingrediente.
9. Los lotes deben priorizarse por fecha de consumo preferente.
10. Las cantidades necesarias de un ingrediente deben consolidarse antes de restar inventario.
11. Una lista de compras debe reflejar únicamente lo que falta.
12. Los ingredientes repetidos deben agruparse.
13. Los precios deben tener fecha y fuente.
14. Los costos históricos deben conservarse.
15. Las compras reales deben asociarse al usuario y presupuesto correspondiente.
16. Los recursos pertenecientes a otros usuarios no deben ser accesibles.
17. Las recetas previamente utilizadas deben preservar su información histórica.
18. Las comidas deben clasificarse según el tipo de comida al que pertenecen.
19. Un usuario no debe tener varios planes activos para la misma semana.
20. Deben existir estados definidos para los menús y sus comidas.

Estados propuestos para el menú:
- DRAFT.
- ACTIVE.
- COMPLETED.
- ARCHIVED.

Estados propuestos para cada comida:
- PLANNED.
- COOKED.
- SKIPPED.

La actualización del inventario cuando se registra una compra y su descuento cuando una comida se marca como cocinada son reglas propuestas en la auditoría, todavía pendientes de aprobación.

No las conviertas en reglas definitivas sin dejar constancia de esta condición.

# 9. MODELO DE DATOS Y ESTRUCTURA LÓGICA

El análisis técnico identifica que el modelo original necesita correcciones para soportar las funcionalidades.

Debes respetar como referencia las siguientes entidades:

- USERS.
- USER_PROFILES.
- DIETARY_TAGS.
- USER_DIETARY_RESTRICTIONS.
- USER_EXCLUDED_INGREDIENTS.
- INGREDIENT_DIET_CONFLICTS.
- INGREDIENTS.
- UNITS.
- INGREDIENT_PRICES.
- INGREDIENT_SUBSTITUTIONS.
- USER_INVENTORY.
- RECIPES.
- RECIPE_MEAL_TYPES.
- RECIPE_INGREDIENTS.
- BUDGETS.
- MEAL_PLANS.
- MEAL_PLAN_ITEMS.
- MEAL_PLAN_ITEM_SUBSTITUTIONS.
- SHOPPING_LISTS.
- SHOPPING_LIST_ITEMS.
- PURCHASES.
- PURCHASE_ITEMS.

Relaciones y consideraciones importantes:

- Un usuario tiene un perfil.
- Un usuario puede tener múltiples restricciones alimentarias.
- Un usuario puede excluir múltiples ingredientes.
- Un ingrediente puede tener diferentes precios registrados.
- Un ingrediente puede aparecer en muchas recetas.
- Una receta puede contener muchos ingredientes.
- Un presupuesto puede financiar menús.
- Un menú contiene múltiples comidas.
- Un menú puede generar una lista de compras.
- Una lista contiene múltiples ingredientes.
- Una compra contiene múltiples productos.
- Una línea de compra puede estar asociada opcionalmente a un ítem de la lista de compras.

No inventes cardinalidades ni relaciones contradictorias.

Respeta las observaciones de la auditoría, especialmente:
- Unidades base.
- Catálogo de conversiones.
- Restricciones alimentarias múltiples.
- Lotes de inventario.
- Costos congelados en los menús.
- Estados de planificación.
- Trazabilidad de compras.
- Sustituciones en una tabla independiente.

En esta etapa utiliza modelos y datos simulados que respeten esa estructura lógica.

# 10. EXPERIENCIA DE USUARIO

Diseña los flujos para que una persona pueda entender la aplicación sin necesitar explicaciones externas.

El flujo principal debe ser:

**Registro → Configuración del perfil → Presupuesto → Inventario → Generación del menú → Revisión → Lista de compras → Registro de compra → Seguimiento.**

El usuario debe tener la posibilidad de omitir el inventario durante el onboarding.

La generación del menú debe ser el punto central de la experiencia.

Evita formularios excesivamente largos.

Divide la información en pasos cuando sea necesario.

Utiliza:
- Mensajes claros.
- Indicadores de progreso.
- Confirmaciones.
- Validaciones inmediatas.
- Estados vacíos con acciones útiles.
- Navegación consistente.
- Acciones principales fácilmente identificables.

# 11. RESPONSIVE Y ACCESIBILIDAD

La aplicación debe funcionar correctamente en:

- Desktop.
- Laptop.
- Tablet.
- Celulares.

Debe contemplar un ancho mínimo de referencia de 360 px.

En escritorio:
- Sidebar lateral.
- Dashboard con distribución de columnas.
- Tablas y calendarios amplios.

En móvil:
- Navegación compacta.
- Tarjetas apiladas.
- Formularios adaptables.
- Menús accesibles.
- Calendario semanal que pueda consultarse sin desbordamiento horizontal innecesario.

Considera WCAG 2.2 nivel AA:
- Contraste adecuado.
- Etiquetas accesibles.
- Navegación por teclado.
- Estados de foco.
- Textos alternativos.
- Mensajes de validación comprensibles.
- Jerarquía semántica.

# 12. CONTENIDO Y DATOS DE DEMOSTRACIÓN

No utilices textos genéricos como "Lorem ipsum".

Crea datos coherentes con el contexto colombiano.

Incluye:
- Ingredientes comunes.
- Recetas colombianas y preparaciones cotidianas.
- Precios de demostración en COP.
- Cantidades y unidades coherentes.
- Presupuestos de ejemplo.
- Inventarios variados.
- Menús semanales completos.

Las cantidades, precios y costos de demostración deben ser consistentes entre inventario, recetas, menú y lista de compras.

No presentes precios simulados como si fueran cotizaciones reales.

No uses recomendaciones médicas ni diagnósticos nutricionales.

# 13. SEGURIDAD Y PRIVACIDAD

Aunque el prototipo utilice datos de demostración, la arquitectura visual y funcional debe contemplar:

- Separación entre USER y ADMIN.
- Protección conceptual de rutas privadas.
- Validación de formularios.
- Separación de datos por usuario.
- Aceptación de términos y tratamiento de datos.
- Eliminación de cuenta.
- Protección de información personal.

Las preferencias alimentarias, alergias e intolerancias pueden constituir información sensible. No expongas estos datos innecesariamente.

No incorpores información real de usuarios.

# 14. FUERA DEL MVP

No desarrolles todavía:

- Aplicación móvil nativa.
- Integración con supermercados.
- Pasarelas de pago.
- Delivery.
- Reconocimiento de alimentos por cámara.
- Escaneo de códigos de barras.
- Predicciones mediante aprendizaje automático.
- Inteligencia artificial avanzada para menús.
- Integración automática con precios externos.
- Funcionalidades médicas o diagnósticas.
- Sustitución avanzada de ingredientes, hasta su aprobación.

No agregues funcionalidades solo porque parezcan interesantes.

# 15. CRITERIOS DE CALIDAD

El resultado debe cumplir lo siguiente:

1. Todas las páginas deben compartir el mismo sistema de diseño.
2. Los botones deben ejecutar acciones reales dentro del prototipo.
3. Los formularios deben validar sus campos.
4. Los cálculos deben ser coherentes.
5. Las cantidades deben respetar las unidades.
6. Los filtros deben funcionar.
7. La navegación debe estar completa.
8. Los estados vacíos deben estar diseñados.
9. Los datos deben ser consistentes entre módulos.
10. No debe existir contenido de demostración contradictorio.
11. Las pantallas deben adaptarse a móviles.
12. Los componentes deben ser reutilizables.
13. No debe haber rutas rotas.
14. No debe haber errores visibles en consola.
15. La interfaz debe parecer un producto real y no una plantilla automática.

# 16. DECISIONES PENDIENTES

El análisis técnico deja ocho decisiones que no deben asumirse como aprobadas:

1. **Viabilidad del presupuesto:** se recomienda medirla con el costo de los ingredientes que faltan por comprar (`estimated_purchase_cost`), no con el costo total de las recetas.
2. **Consumo del inventario:** se propone descontarlo al marcar una comida como COOKED.
3. **Sustituciones:** se recomienda incluir cambio de receta en el MVP y diferir sustitución de ingredientes.
4. **Recuperación de contraseña:** se recomienda diferirla porque requiere servicio de correo.
5. **Interfaz:** se recomienda utilizar estilos propios y design tokens, evitando Bootstrap.
6. **Despliegue y equipo:** todavía no están definidos.
7. **Contenido:** se propone comenzar con entre 40 y 60 recetas y definir quién administra recetas y precios.
8. **Idioma:** se recomienda utilizar identificadores de código en inglés e interfaz en español.

Utiliza los puntos anteriores como decisiones provisionales para el prototipo y explícita cualquier comportamiento que dependa de ellos.

# 17. FORMA DE TRABAJO

No intentes construir toda la aplicación en una sola operación sin planificación.

Trabaja por etapas:

**ETAPA 1. Planificación**
- Lee los documentos.
- Analiza los requisitos.
- Propón arquitectura de interfaz.
- Define las rutas.
- Define los componentes.
- Define los modelos de datos simulados.
- Identifica decisiones pendientes.
- Presenta un plan de implementación.

**ETAPA 2. Sistema visual y estructura**
- Define tokens.
- Crea componentes base.
- Diseña navegación.
- Construye layout público y privado.
- Implementa responsive.

**ETAPA 3. Flujos principales**
- Onboarding.
- Dashboard.
- Presupuesto.
- Inventario.
- Recetario.

**ETAPA 4. Funcionalidad principal**
- Generador de menús.
- Calendario semanal.
- Detalle de comidas.
- Lista de compras.

**ETAPA 5. Seguimiento**
- Registro de compras.
- Control de gastos.
- Historial.

**ETAPA 6. Administración**
- Recetas.
- Ingredientes.
- Precios.

**ETAPA 7. Validación**
- Revisión visual.
- Revisión de flujos.
- Validación de cálculos.
- Pruebas responsive.
- Pruebas de accesibilidad.
- Corrección de errores.

Al finalizar cada etapa, conserva lo que ya funciona y evita modificar componentes o módulos no relacionados con el cambio solicitado.

# 18. INSTRUCCIÓN INICIAL

Por ahora, trabaja únicamente en la **ETAPA 1: PLANIFICACIÓN**.

No generes código todavía.

Quiero que primero:

1. Analices el SRS v1.0.
2. Analices el documento de auditoría técnica.
3. Identifiques los módulos que debe tener la aplicación.
4. Definas la arquitectura de navegación.
5. Propongas las pantallas necesarias.
6. Definas los componentes reutilizables.
7. Propongas la organización del proyecto.
8. Identifiques las funcionalidades que necesitan datos simulados.
9. Identifiques los puntos que requieren confirmación.
10. Presentes un plan de construcción por etapas.

No elimines requisitos ni simplifiques el producto sin justificarlo.

**Espera mi aprobación del plan antes de comenzar a generar la aplicación.**

El objetivo final es obtener un prototipo de NutriBudget que represente fielmente el producto especificado, tenga una experiencia de usuario profesional y permita validar su funcionamiento antes de implementar el sistema definitivo con Angular, Spring Boot y PostgreSQL.

# NutriBudget — Etapa 1: Plan del prototipo

> Nota: solo recibí el prompt maestro. El **SRS v1.0** y el **análisis de auditoría** no venían adjuntos. Este plan se basa en lo que el prompt resume de ambos; si los subes, ajusto el plan antes de empezar.

## 1. Módulos

| # | Módulo | Requisitos | Tipo |
|---|---|---|---|
| 0 | Sitio público | — | Definido |
| 1 | Autenticación y cuenta | RF-01, RF-02, RF-20 | Definido |
| 2 | Onboarding y perfil alimentario | RF-03, RF-05 | Definido |
| 3 | Dashboard | RF-21 | Propuesta auditoría |
| 4 | Presupuesto | RF-04 | Definido |
| 5 | Inventario (lotes) | RF-06, RF-07 | Definido + corrección auditoría |
| 6 | Recetario | RF-08 | Definido |
| 7 | Planificador / generador | RF-09 a RF-12 | Definido + reglas auditoría |
| 8 | Lista de compras | RF-13 | Definido |
| 9 | Compras y gastos | RF-14 a RF-16 | Definido |
| 10 | Historial | — | Definido |
| 11 | Administración | Roles USER/ADMIN | Definido |

## 2. Arquitectura de navegación

```text
Público            /  ·  /registro  ·  /ingresar  ·  /terminos  ·  /privacidad
Onboarding         /onboarding   (pasos 1-3 con indicador de progreso)
App (USER)         /app                      Dashboard
                   /app/presupuesto
                   /app/inventario
                   /app/recetas  ·  /app/recetas/:id
                   /app/planificador         (configurar + calendario)
                   /app/planificador/:mealId (detalle de comida)
                   /app/lista-compras
                   /app/gastos  ·  /app/gastos/nueva
                   /app/historial  ·  /app/historial/:planId
                   /app/perfil               (preferencias, eliminar cuenta)
Admin (ADMIN)      /admin  ·  /admin/recetas  ·  /admin/recetas/:id
                   /admin/ingredientes  ·  /admin/precios
```

- Protección conceptual: sesión simulada. Sin sesión → `/ingresar`. Perfil incompleto → `/onboarding`. USER que entra a `/admin` → redirección con aviso.
- En `/ingresar` habrá accesos rápidos "Entrar como usuario demo" y "Entrar como administrador demo".
- Escritorio: barra lateral + cabecera con avatar y accesos rápidos. Móvil (desde 360 px): barra inferior con 5 accesos principales + menú "Más".

## 3. Pantallas y estados clave

| Pantalla | Contenido principal | Estados |
|---|---|---|
| Inicio público | Hero, cómo funciona (4 pasos), beneficios, funcionalidades, ahorro y desperdicio, llamado a registrarse, footer | — |
| Registro / Ingreso | Validación inmediata, términos + tratamiento de datos (`terms_accepted_at`), "¿Olvidaste tu contraseña?" deshabilitado como "Próximamente" | Error, cargando |
| Onboarding | Paso 1 hogar y 4 categorías separadas; paso 2 presupuesto y fechas; paso 3 inventario omitible | Validación, confirmación |
| Dashboard | Presupuesto, próxima comida, menú del día, inventario por vencer, compras pendientes, mensajes guía | Vacío sin configuración |
| Presupuesto | Crear/editar, estimado vs. real, saldo, % usado | Error por solapamiento o valor ≤ 0 |
| Inventario | Lotes por ingrediente, búsqueda, filtro por categoría, orden por fecha, pestañas Disponibles / Por consumir / Agotado | Vacío, confirmar eliminación |
| Recetario + detalle | Tarjetas con foto, filtros (comida, tiempo, ingrediente, categoría, preferencia, costo), detalle con ingredientes, pasos y costo | Sin resultados |
| Planificador | Configuración → generación → calendario semana × comida, desglose de 5 costos, cambiar receta, regenerar, faltantes/disponibles | Cargando, plan supera presupuesto, sin recetas compatibles |
| Lista de compras | Agrupada por ingrediente, necesario / en casa / falta, subtotal, casillas, filtros, estado | Vacía sin menú |
| Gastos / nueva compra | Registro con valor real por línea (`line_total`), vinculación opcional a la lista, compra parcial, gráfica estimado vs. real | Vacío, confirmación |
| Historial | Menús, presupuestos, compras, evolución, costos congelados | Vacío |
| Perfil | Datos, preferencias, alergias, exclusiones, eliminar cuenta (doble confirmación) | Confirmación |
| Admin | Tablas CRUD de recetas, ingredientes (unidad base, categoría, grupo, conflictos) y precios (fuente, fecha, alerta de desactualizado) | Vacío, validación |

## 4. Componentes reutilizables

- **Base:** Botón (primario, secundario, fantasma, peligro), campo, selector, casilla, chips de selección, modal, aviso emergente, alerta, etiqueta de estado, tarjeta, pestañas, indicador de pasos, barra de progreso, estado vacío, esqueleto de carga, tabla.
- **Formato:** `Money` ($ 150.000 COP), `Quantity` (conversión g↔️kg, ml↔️L), `DateLabel`, `ProvisionalNote` (marca visible de comportamientos pendientes de aprobación), `EstimatedPriceNote`.
- **Estructura:** cabecera y footer públicos, barra lateral de la app, cabecera de la app, navegación móvil, barra lateral de admin.
- **Dominio:** tarjeta de presupuesto, tarjeta de receta, filtros de receta, fila de lote, etiqueta de vencimiento, calendario semanal, casilla de comida, modal de cambio de receta, desglose de costos, fila de lista de compras, formulario de compra, gráfica estimado vs. real.

## 5. Datos simulados

- Catálogo: ~45 ingredientes colombianos con unidad base, categoría, grupo alimentario y precio de ejemplo con fuente "Estimación de demostración" y fecha.
- 12 recetas del prompt (arepa con huevo, avena, arroz con pollo, lentejas, sudado, ensalada de garbanzos, tortilla de vegetales, pasta con verduras, fríjoles, sopa de verduras, arroz con huevo, crema de ahuyama) con foto generada, porciones, pasos, etiquetas y conflictos.
- Etiquetas: vegetariano, sin gluten, sin lactosa, alergia al huevo, al maní, a mariscos, etc.
- Usuario demo "Laura" (hogar de 2, $ 150.000 COP semanales, 10 lotes de inventario, algunos por vencer), un menú activo, una lista generada, 2 compras registradas, 3 semanas de historial. Un admin demo.
- Todas las cifras se derivan de las mismas funciones de cálculo, para que coincidan entre módulos.

## 6. Generador de menús (reglas, sin IA)

1. Filtrar recetas incompatibles con alergias, restricciones y exclusiones (a través de los conflictos entre ingredientes y etiquetas).
2. Puntuar: uso de ingredientes por vencer, costo de compra faltante, variedad (sin repetir receta en el mismo día ni más de 2 veces por semana) y balance de grupos.
3. Llenar las casillas día × comida de forma voraz respetando el presupuesto; el resultado es determinístico (regenerar = otra semilla).
4. Consolidar la necesidad total por ingrediente en su unidad base → descontar inventario **una sola vez**, primero los lotes que vencen antes → lista de compras con solo lo que falta.
5. Escalar por número de personas versus las porciones de la receta.

## 7. Puntos que requieren tu confirmación

| Decisión pendiente | Comportamiento provisional en el prototipo |
|---|---|
| Viabilidad del presupuesto | Medida con `estimated_purchase_cost`, señalada con `ProvisionalNote` |
| Descontar inventario al marcar COOKED | Acción opcional con confirmación y nota "provisional" |
| Sumar a inventario al registrar compra | Casilla "Agregar sobrante al inventario", marcada como provisional |
| Sustituciones | Solo cambio de receta; sustitución de ingredientes no se construye |
| Recuperación de contraseña | Enlace visible deshabilitado "Próximamente" |
| Comidas a planificar | Desayuno, almuerzo y cena, configurables por el usuario |
| Cantidad de recetas | 12 en la demo (la auditoría propone 40–60) |
| Idioma | Interfaz en español, identificadores en inglés |
| Despliegue y equipo | Fuera del alcance del prototipo |

## 8. Construcción por etapas

1. **Etapa 2 — Sistema visual y estructura:** colores y tipografías oficiales, componentes base, estructura pública/app/admin, navegación responsive, sesión demo y protección de rutas, sitio público completo.
2. **Etapa 3 — Flujos principales:** registro, ingreso, onboarding, dashboard, presupuesto, inventario, recetario + detalle (con fotos generadas).
3. **Etapa 4 — Funcionalidad central:** generador, calendario semanal, detalle de comida, cambio de receta, lista de compras.
4. **Etapa 5 — Seguimiento:** registro de compras, control de gastos, historial.
5. **Etapa 6 — Administración:** recetas, ingredientes, precios.
6. **Etapa 7 — Validación:** pruebas automáticas de reglas, revisión visual en 360/768/1280 px, teclado y contraste, consola sin errores.

Al terminar cada etapa me detengo para que la revises.

## Detalles técnicos

- Stack de Lovable: TanStack Start (React 19 + TypeScript + Tailwind v4). Esto **no** es Angular; la arquitectura final (Angular + Spring Boot + PostgreSQL) se respeta.
- Estructura portable:
  - `src/domain/models/` — tipos que reflejan las 23 entidades (User, UserProfile, DietaryTag, UserDietaryRestriction, UserExcludedIngredient, IngredientDietConflict, Ingredient, Unit, IngredientPrice, UserInventory, Recipe, RecipeMealType, RecipeIngredient, Budget, MealPlan, MealPlanItem, ShoppingList, ShoppingListItem, Purchase, PurchaseItem…). `IngredientSubstitution` y `MealPlanItemSubstitution` solo como tipos.
  - `src/domain/rules/` — funciones puras (unidades, generador, consolidación, costos, validaciones), trasladables a servicios Java.
  - `src/services/` — repositorios simulados asíncronos con firmas parecidas a endpoints REST, latencia y errores simulables, persistencia en el navegador (localStorage) y botón "Restablecer datos demo".
  - `src/mocks/` — datos semilla. `src/components/{ui,layout,<módulo>}`. `src/routes/`.
- Estado: TanStack Query sobre los servicios; sesión simulada con rol.
- Sin Lovable Cloud ni otro backend hasta que lo autorices.
- Pruebas unitarias (Vitest) para: no duplicar descuento de inventario, orden por vencimiento, exclusión por alergias, conversión de unidades, cálculos de presupuesto y solapamiento de presupuestos.