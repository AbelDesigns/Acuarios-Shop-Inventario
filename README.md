# Acuarios Shop — Inventario y Ventas

Aplicación web con sincronización en tiempo real en **Cloud Firestore** y acceso protegido con **Firebase Authentication** para la gestión diaria de **Acuarios Shop**:

- **1. Vender (Caja Rápida):** carrito de compras, facturación en Dólares (`$`) y Bolívares (`Bs`), formas de pago, devolución/anulación atómica de ventas y cierre diario copiable para WhatsApp.
- **2. Inventario:** control de stock en tiempo real entre dispositivos, alertas de pocas unidades/agotadas, edición rápida y exportación a CSV (Excel).
- **3. Ropa Nueva:** alta individual o por lote surtido de tallas/colores con compresión automática de fotos y calculadora de costo/margen.
- **4. Tasas del Día:** gestión sincronizada de tasas (BCV, Euro BCV, Binance USDT y Promedio) con conversor instantáneo.

## Seguridad y Firebase

- **Proyecto Firebase:** `acuariosshop-731c5` (Cloud Firestore con caché offline + Firebase Auth).
- **Control de acceso estricto (`firestore.rules`):** solo cuentas autenticadas con correo verificado y activas en la colección `authorizedUsers` pueden leer o escribir datos.
- **Gestión de equipo:** el administrador puede autorizar, pausar o revocar correos desde el botón **Equipo** dentro de la app.
- **Publicación:** https://abeldesigns.github.io/Acuarios-Shop-Inventario/
