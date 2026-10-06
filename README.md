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

## ☕ Historias de Usuario 

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


