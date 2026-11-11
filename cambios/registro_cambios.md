titulo <<Registro de cambios>>
# Registro de solicitudes de cambio – VentasNet

## Solicitud 1: INC-001

* ID: INC-001
* Origen: Incidencia detectada durante la revision del sistema.
* Descripcion: El total de la venta no considera la cantidad de productos ingresada.
* Justificacion: Corregir el calculo del importe total para que el sistema multiplique correctamente el precio unitario por la cantidad de productos.
* Requisito afectado: RF-001.
* Archivos involucrados: src/ventas.py
* Riesgo: Mostrar importes incorrectos y generar errores en las ventas.
* Criterio de aceptacion: Si el precio unitario es S/ 50 y la cantidad es 3, el sistema debe calcular un total de S/ 150.
* Prioridad: Alta.
* Decision: Aprobada para correccion.
* Responsable: Equipo de desarrollo.
# MATRIZ DE IMPACTO 
* Requisito: RF-001
* Archivo: src/ventas.py
* Riesgo: Total incorrecto
* Prueba: 50 x 3 = 150
* Decision simulada: implementada y verificada

---

## Solicitud 2: CR-002

* ID: CR-002
* Origen: Solicitud de mejora funcional.
* Descripcion: Implementar un descuento del 10 % cuando el subtotal de la compra sea igual o superior a S/ 200.
* Justificacion: Incorporar una promocion que beneficie a los clientes y mejore la funcionalidad del sistema.
* Requisito afectado: implementar el requisito <<RF-002: Aplicar 10 % de descuento cuando el subtotal sea igual o 
superior a S/ 200>>
* Archivos involucrados: src/ventas.py
* Riesgo: Aplicar descuentos incorrectos o afectar el calculo del importe final.
* Criterio de aceptacion:
  * Si el subtotal es S/ 200, aplicar el 10 % de descuento y obtener S/ 180.
  * Si el subtotal es S/ 150, no aplicar descuento y mantener S/ 150.
* Prioridad: Media.
* Decision: Aprobada para implementaciOn.
* Responsable: Equipo de desarrollo.
# MATRIZ DE IMPACTO 
* Requisito: RF-002(nuevo)
* Archivo: src/ventas.py; docs/requisitos.md
* Riesgo: Descuento incorrecto en umbral 
* Prueba: Subtotales 150, 200 y 300 
* Decision simulada: Aprobada
----------------
