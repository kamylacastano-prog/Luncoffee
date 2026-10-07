# Luncoffee

## **Introducción**
El presente proyecto tendrá como propósito analizar, diseñar y desarrollar un sistema de información para optimizar los procesos administrativos de la cafetería del SENA. La información se obtendrá mediante entrevistas, observación directa y análisis de los procesos actuales. Con base en los resultados, se diseñará e implementará una solución tecnológica.

## **Planteaminento del problema**
La cafetería del SENA presenta dificultades en la gestión de inventarios, ventas, pedidos y reportes, debido al manejo poco organizado de la información. Esto puede generar errores, pérdida de datos y retrasos en los procesos administrativos. Por esta razón, se propone desarrollar un sistema de información que permita organizar y optimizar estos procesos, facilitando la gestión y la toma de decisiones.

## **Justificacion**
El desarrollo de este proyecto permitirá modernizar la gestión administrativa de la cafetería mediante la implementación de un sistema de información. Se espera reducir errores en los registros, optimizar el control del inventario, agilizar la atención al cliente y mejorar la administración de los recursos. Además, el proyecto fortalecerá las competencias adquiridas durante la formación en Análisis y Desarrollo de Software.

## 🌳 **Arbol de problemas**  

### 1️⃣ Problema Central (Tronco)
Deficiente e ineficiente sistema actual de gestión de ventas, caja e inventarios en los puntos de producción (Don Bosco, El Vagón y La Cafetería).

### 2️⃣ Causas (Raíces)
**Causas Directas (Nivel 1):**  

 - **Herramienta operativa limitada e inalterable: Uso de un libro de Excel elemental y bloqueado para el registro de ventas.**

 - **Proceso de validación de pagos lento: Verificación manual de pagos por transferencia (QR / Bre-B) mediante captura de fotos.**

 - **Ausencia de un control de inventarios automatizado: Inexistencia de un sistema que descuente automáticamente insumos según las ventas realizadas.**

 - **Falta de integración y automatización en el flujo de pedidos: Comunicación verbal/manual de los pedidos entre la caja y la zona de preparación (baristas/cocina).**

 - **Gestión inflexible de productos y precios de panadería: Dificultad para actualizar diariamente el menú variable y los costos cambiantes de la producción académica.**
   
**Causas Indirectas (Nivel 2):**
 - **La plantilla de Excel actual no permite modificar celdas por estar bloqueada, impidiendo ajustar precios o insumos que cambian con frecuencia.**

 - **Rotación constante del personal (3 cajeros por día, aprendices y pasantes) que genera demoras al reingresar datos repetidos (ej. nombre del cajero por transacción).**

 - **Inexistencia de un sistema de comandas automáticas que envíe la orden a preparación de forma simultánea al pago.**

 - **Falta de recetas estándar integradas al software para el descuento en tiempo real de insumos clave (café, leche, azúcar, empaques).**

 - **Ausencia de alertas automáticas para el reabastecimiento por punto de stock mínimo.**
   
### 3️⃣ Efectos y Consecuencias (Ramas y Hojas)
**Efectos Directos (Nivel 1):**
 - **Demoras y cuellos de botella en la atención al cliente: Tiempos de espera prolongados mientras se valida la transacción por QR o se busca el producto en la lista de Excel.**

 - **Reprocesos operativos en los cierres de caja: Inconsistencias al revisar fotos de comprobantes e imprimir tirillas para conciliar las ventas diarias de los tres turnos.**

 - **Riesgo de desabastecimiento de insumos: Posibilidad de quedarse sin stock crítico por falta de un sistema preventivo de alertas de inventario.**

 - **Vulnerabilidad en la seguridad del sistema: Riesgo de alteraciones indebidas en las ventas o eliminaciones sin autorización de administradores/supervisores.**

 - **Dificultad para coordinar distintas sedes/módulos: Problemas al adaptar la misma herramienta a dinámicas variadas (ej. gestión de mesas en El Vagón vs. atención de barra en Don Bosco).**

**Efectos Indirectos / Impacto Final (Nivel 2):**
- **Pérdida de eficiencia académica y productiva en los ambientes de formación real.**

- **Inconformidad de los clientes (estudiantes y usuarios) por filas largas e ineficiencia en el servicio.**

- **Falta de trazabilidad y datos fiables para la toma de decisiones administrativas en el área de economato y gestión de producción.**

---

## 🌳 Árbol de Objetivos

### 1️⃣ Objetivo Central (Tronco)
* Implementar un sistema de información eficiente y automatizado para la gestión de ventas, caja e inventarios en los puntos de producción de la cafeterias.

### 2️⃣ Medios / Alternativas de Solución (Raíces)

#### Medios Directos:
* **Sustitución del sistema actual:** Desplegar un software amigable, flexible y configurable en reemplazo del archivo de Excel elemental y bloqueado.
* **Agilización de pagos:** Automatizar la validación y registro de pagos digitales por transferencias registrando el código/dígito de comprobante.
* **Control de stock automático:** Implementar un control de inventarios automatizado que descuente materias primas en tiempo real mediante recetas estándar.
* **Integración de pedidos:** Integrar la emisión de comandas automáticas a la zona de preparación (barra/cocina) de forma simultánea al cobro.
* **Menú dinámico:** Habilitar un módulo de creación y modificación dinámica de productos y precios diarios para la oferta variable de panadería.

#### Medios Indirectos:
* Interfaz intuitiva que permita actualizar catálogo y tarifas sin requerir modificaciones en código o celdas protegidas.
* Asignación automática del cajero activo en turno para agilizar el flujo ante la rotación de aprendices y pasantes.
* Configuración de impresoras independientes en la zona de producción para recibir comandas sin depender de comunicación verbal.
* Vinculación de recetas estándar de bebidas (gramos de café, mililitros de leche, salsa, azúcar) al catálogo.
* Sistema de notificaciones en pantalla por stock mínimo.

### 3️⃣ Fines e Impactos Positivos (Ramas y Hojas)

#### Fines Directos:
* **Reducción de tiempos de espera:** Agilización en la atención al cliente y eliminación de filas en horas pico.
* **Precisión operativa:** Conciliación y cierre de caja rápido y preciso al finalizar los turnos.
* **Prevención de desabastecimiento:** Alertas preventivas de stock mínimo para evitar desabastecimiento de insumos clave.
* **Seguridad y auditoría:** Control de acceso basado en roles que prevenga eliminaciones no autorizadas.
* **Adaptabilidad:** Flexibilidad para configurar módulos según la sede (ej. gestión de mesas en *El Vagón* vs. venta rápida de barra en *Don Bosco*).

#### Fines Indirectos / Impacto Final :
* Optimización de la eficiencia académica y operativa en los ambientes de formación real del SENA.
* Mayor satisfacción de los usuarios (estudiantes, instructores y visitantes).
* Disponibilidad de datos e informes fiables para la toma de decisiones en el economato y la administración general.

---

## 🎯 Objetivo General

Diseñar, desarrollar e implementar un sistema de información web/escritorio (POS e inventarios) para las cafeterias, que optimice y automatice los procesos de ventas, control de caja, gestión de inventarios por recetas estándar y comandas en sus diferentes centros de producción.

---

## 📌 Objetivos Específicos

1. **Módulo POS y Facturación Ágil:** Diseñar una interfaz táctil en cuadrícula optimizada para el registro de ventas sin efectivo (pagos por transferencia), asignando automáticamente el cajero activo por turno.
2. **Gestión de Comandas Independientes:** Habilitar el envío simultáneo de la orden a la zona de preparación (barra/cocina) de forma paralela o previa a la validación del pago.
3. **Inventarios con Recetas Estándar:** Automatizar el descuento de insumos (café, leche, azúcar, empaques) en tiempo real al vender bebidas estandarizadas e integrar el ingreso directo por unidades para productos de panadería y repostería variable.
4. **Alertas de Stock Mínimo y Entradas:** Permitir la notificación preventiva en pantalla cuando un insumo alcance su límite crítico y registrar el ingreso de materias primas provenientes del economato.
5. **Cierres de Caja por Turnos:** Automatizar la generación de reportes e impresión de tirillas de cierre para los tres turnos de atención diaria (8:00 am–12:00 pm, 12:00 pm–4:00 pm y 4:00 pm–8:00 pm), desglosando ventas por cajero y plataforma de pago.
6. **Seguridad y Adaptabilidad Modular:** Implementar control de acceso basado en roles (Cajero/Aprendiz vs. Administrador/Supervisor) con autorización para anulaciones, así como la habilitación/deshabilitación modular de funciones según el punto operativo.

---

## 📐 Alcance del Proyecto

### Detalle del Alcance

#### Funcionalidades Incluidas:
* **Módulo POS Táctil:** Interfaz amigable para la selección rápida de productos y cantidades, con soporte de hasta 3 cierres de caja al día y asignación dinámica del cajero activo.
* **Módulo de Comandas Independientes:** Envío automático de comandas a la zona de preparación (vía impresora térmica o pantalla de producción) de forma paralela al cobro.
* **Módulo de Métodos de Pago Digitales:** Registro exclusivo de transferencias mediante la infraestructura *Bre-B / QR* (Nequi, Bancolombia, Nu, Banco de Bogotá, Davivienda, etc.), incluyendo un campo obligatorio para registrar el código/dígito del comprobante de transferencia.
* **Módulo de Inventario Dinámico y Recetas Estándar:** Descuento automático proporcional de insumos según recetas estándar para bebidas e ingreso directo por unidades para productos de producción académica variable en panadería/repostería.
* **Control de Stock Mínimo y Entradas:** Alerta en pantalla al alcanzar el nivel crítico de insumos y formulario para el ingreso de requisiciones o materias primas.
* **Seguridad y Roles de Usuario:** Restricción estricta de permisos para que el perfil "Cajero" no pueda borrar ni anular ventas sin autorización o clave del perfil "Administrador".
* **Configuración Modular por Sede:** Funcionalidad para activar o desactivar módulos según el centro operativo (ej. activar gestión de hasta 15 mesas en *El Vagón* o desactivarla para atención exclusiva en barra en *Don Bosco*).
* **Módulo opcional de Clientes:** Formulario de consulta/registro rápido de clientes por cédula para recolección de datos analíticos.

#### Exclusiones del Sistema:
* **Pagos en efectivo:** El software omite totalmente la opción de cobro físico o gestión de dinero en efectivo por políticas institucionales de la cafetería.
* **Inventario de insumos de producción académica en aulas:** No se controlarán los ingredientes crudos (harina, levadura, mantequilla) utilizados dentro de los talleres de formación de panadería.
* **Facturación electrónica DIAN / Impuestos complejos:** No se incluyen retenciones ni liquidación de IVA, ya que corresponde a un modelo simplificado de venta interna en ambiente de aprendizaje.
* **Servicio de domicilios o pedidos externos:** El sistema está acotado exclusivamente a la venta presencial dentro de las instalaciones y sedes del SENA.

---

## Historias de Usuario 

Este documento contiene la especificación de Historias de Usuario (HU) estructuradas para el desarrollo del software del punto de venta.

---

---

## 📂 Módulo 1: Gestión de Catálogo y Menú Variable

### 📄 HU-01: Registro y Modificación Dinámica de Productos
* **Como:** 👤 Cajero / Administrador
* **Quiero:** 🥐 Crear, modificar o actualizar productos del menú (especialmente de panadería/repostería) y sus precios de forma rápida 
* **Para:** 📈 Adaptar la oferta diaria según la disponibilidad de la práctica de los aprendices (ej. tiramisú, croissants, pañuelos) 

#### ⚙️ Criterios de Aceptación
-  Permite agregar un producto temporal o modificar un precio existente.
-  Interfaz táctil/visual mediante botones/cuadros seleccionables con imágenes o accesos directos (evitar listas desplegables complejas).

---

## 📂 Módulo 2: Facturación, Ventas y Métodos de Pago

### 📄 HU-02: Registro de Ventas Ágil
* **Como:** 👤 Cajero
* **Quiero:** 👆 Seleccionar productos de forma táctil e ingresar la cantidad requerida .
* **Para:** ⚡ Agilizar la atención al cliente y evitar filas en el punto de venta .

#### ⚙️ Criterios de Aceptación
-  Interfaz optimizada por bloques o categorías visuales.
-  Asignación automática del cajero activo al ticket sin solicitar su nombre en cada transacción.

### 📄 HU-03: Procesamiento de Pagos Digitales (Llaves / Transferencias)
* **Como:** 👤 Cajero
* **Quiero:** 📱 Registrar pagos exclusivamente por medios digitales (Nequi, Bancolombia, Nu, Davivienda, etc.).
* **Para:** 🛡️ No manejar dinero en efectivo dentro del establecimiento .

#### ⚙️ Criterios de Aceptación
-  El sistema bloquea y no permite seleccionar la opción "Pago en Efectivo".
-  Incluye un campo obligatorio para asociar/adjuntar el comprobante o dígito de verificación del pago.

### 📄 HU-04: Emisión de Comanda y Factura Simple
* **Como:** 👤 Cajero
* **Quiero:** 🖨️ Generar de forma independiente la comanda de preparación y la factura del cliente .
* **Para:** ⏱️ Que la cocina o barra comience la preparación del pedido inmediatamente sin esperar a que finalice la validación del pago .

#### ⚙️ Criterios de Aceptación
-  Envío automático de la comanda a la impresora del área de producción correspondiente (bebidas/alimentos).
-  Emisión de una factura básica para el cliente (sin retenciones ni impuestos).

---

## 📂 Módulo 3: Control de Inventario y Recetas Estándar

### 📄 HU-05: Descuento Automático por Receta Estándar (Bebidas/Insumos)
* **Como:** 👤 Administrador
* **Quiero:** 📋 Asociar recetas estándar a las bebidas (ej. gramos de café, leche, azúcar por capuchino).
* **Para:** 📉 Que el inventario de insumos se descuente automáticamente con cada venta realizada .

#### ⚙️ Criterios de Aceptación
-  Al vender un producto con receta, se descuentan las cantidades proporcionales en el stock de insumos básicos.
-  Los productos terminados (panadería/repostería) descuentan stock por unidades simples (1 a 1).

### 📄 HU-06: Alertas de Stock Mínimo
* **Como:** 👤 Cajero / Administrador
* **Quiero:** ⚠️ Recibir una notificación en pantalla cuando un insumo o producto alcance su límite mínimo.
* **Para:** 🛒 Realizar la requisición de reabastecimiento a tiempo sin interrumpir la operación de venta.

#### ⚙️ Criterios de Aceptación
-  Mostrar una alerta visual clara en la interfaz del punto de venta (POS).
-  Permitir seguir facturando hasta que el stock llegue a cero si el administrador así lo configura.

### 📄 HU-07: Registro de Entradas e Insumos
* **Como:** 👤 Administrador / Encargado de Insumos
* **Quiero:** 📦 Registrar la entrada de materias primas que llegan al centro (ej. kilos de café, bolsas de leche).
* **Para:** 🔄 Mantener actualizado el inventario real del sistema.

#### ⚙️ Criterios de Aceptación
-  Formulario de entrada que sume las nuevas existencias al stock actual con fecha y responsable.

---

## 📂 Módulo 4: Cierre de Caja y Reportes

### 📄 HU-08: Cierre de Caja por Turno / Cajero
* **Como:** 👤 Cajero
* **Quiero:** 🔒 Realizar un cierre parcial o final al terminar mi turno de trabajo.
* **Para:** 📊 Conciliar mis ventas registradas con los comprobantes de pago digital recibidos.

#### ⚙️ Criterios de Aceptación
-  Soporte para múltiples cierres programados al día (ej. 8:00-12:00, 12:00-16:00, 16:00-20:00).
-  Imprimir o generar un reporte exportable con el detalle de ventas, hora, productos y desglose por método de pago.

---

## 📂 Módulo 5: Roles, Permisos y Configuración de Sede

### 📄 HU-09: Control de Acceso y Modificación de Cuentas
* **Como:** 👤 Administrador
* **Quiero:** 🚫 Restringir el permiso de anulación o eliminación de facturas/ventas únicamente a usuarios autorizados.
* **Para:** 🔐 Evitar pérdidas o modificaciones no autorizadas por parte de los cajeros/aprendices.

#### ⚙️ Criterios de Aceptación
-  El perfil "Cajero" solo tiene permisos para registrar ventas y comandar.
-  Se requiere una autorización en pantalla o clave de Administrador para eliminar o editar un ticket ya emitido.

### 📄 HU-10: Configuración por Punto / Sede (Módulo de Mesas Opcional)
* **Como:** 👤 Administrador
* **Quiero:** ⚙️ Habilitar o deshabilitar módulos específicos según la sede (ej. activar gestión de mesas en "El Vagón" y desactivarla en "Don Bosco").
* **Para:** 🏢 Usar la misma aplicación base en diferentes tipos de centros de formación/producción.

#### ⚙️ Criterios de Aceptación
- Posibilidad de activar o desactivar la vista gráfica de mesas (hasta 15 mesas/barra) según el perfil de la sede seleccionada.

---

## 📂 Módulo 6: Fidelización / Registro de Clientes (Opcional / Deseable)

### 📄 HU-11: Registro y Búsqueda de Clientes
* **Como:** 👤 Cajero
* **Quiero:** 🔍 Consultar o registrar datos básicos de clientes (cédula, nombre, teléfono) al momento de la venta.
* **Para:** 🗂️ Estructurar una base de datos analítica de usuarios de la cafetería.

#### ⚙️ Criterios de Aceptación
- [ ] Buscador rápido por número de cédula en la pantalla principal de facturación.
-  Formulario ágil para crear un cliente nuevo sin abandonar el flujo de la venta actual.


