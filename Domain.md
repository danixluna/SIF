# Sistema de Administración Financiera Personal
## Modelo de Dominio (Borrador v0.2)
# Nueva entidad: Contraparte
Representa cualquier persona o entidad con la que existe una relación financiera.
## Información
- Identificador
- Nombre
- Alias
- Tipo
- RFC (opcional)
- Teléfono (opcional)
- Correo (opcional)
- Notas
Tipos sugeridos:
- Familiar
- Amigo
- Conocido
- Empresa
- Comercio grande
- Comercio pequeño
- Gobierno
- Institución financiera
- Empleador
- Cliente
- Proveedor
- Otro
---
# Evolución de Cuenta → Producto Financiero
## Tipos
### Cuentas
- Débito
- Cheques
- Ahorro
- Inversión
- Efectivo
- Cuenta puente
### Productos de crédito
- Tarjeta de crédito
- Crédito personal
- Crédito automotriz
- Crédito hipotecario
- Crédito de nómina
- Crédito departamental
- Línea de crédito revolvente
Información común
- Identificador
- Nombre
- Banco
- Titular
- Estado
- Saldo
- Fecha de apertura
---
# Información específica para créditos
## Tarjetas de crédito
- Límite de crédito
- Crédito disponible
- Crédito utilizado
- Fecha de corte
- Fecha límite de pago
- Pago mínimo
- Pago para no generar intereses
- Tasa
- CAT (opcional)
## Créditos
- Monto contratado
- Saldo pendiente
- Número de pagos
- Pago periódico
- Fecha de contratación
- Fecha de vencimiento
- Tasa
- Tipo de interés
---
# Actualización de Tarjetas
Información
- Producto financiero asociado
- Banco emisor
- Terminación
- Número completo (opcional)
- Usuario asignado
- Física / Virtual
- Estado
---
# Actualización de Transacciones
## Medio de operación
Si se utiliza tarjeta:
- Tarjeta presente
- Tarjeta no presente
## Estados
- Borrador
- Programada
- Pendiente
- Aplicada
- Cancelada
- Revertida
---
# Compras parcializadas
Una transacción puede generar una parcialización.
Información
- Transacción origen
- Total de pagos
- Pago actual
- Importe por pago
- Fecha del siguiente cargo
- Frecuencia
- Tipo
Tipos
- Meses sin intereses
- Parcialización con intereses
- Compra diferida
Indicadores
- Genera intereses
- Tasa
- Total intereses
- Total a pagar
- Estado
---
# Presupuesto
Representa la planeación financiera del usuario.
Agrupa conceptos presupuestales.
---
# Concepto Presupuestal
Representa un compromiso o movimiento esperado.
Ejemplos
- Spotify
- Internet
- Renta
- Pago de tarjeta
- Nómina
- Seguro
- Ahorro
## Información
- Identificador
- Nombre
- Tipo
- Categoría
- Importe esperado
- Frecuencia
- Fecha esperada
- Producto financiero sugerido
- Contraparte
- Prioridad
- Activo
Tipos
- Servicio
- Deuda
- Ingreso esperado
- Ahorro programado
- Gasto fijo
- Gasto variable esperado
Cada concepto podrá generar transacciones programadas que posteriormente serán confirmadas.
---
# Relación conceptual
Usuario
↓
Presupuesto
↓
Concepto Presupuestal
↓
Transacción Programada
↓
Transacción Aplicada
---
# Pendientes
- Modelo completo de presupuestos.
- Metas de ahorro.
- Gestión de inversiones.
- Gestión de deudas.
- Conciliación bancaria.
- Importación de estados de cuenta.
- Reglas automáticas de categorización.
- Dashboard financiero.
- Objetivos financieros.
- Patrimonio (activos y pasivos).
- Gestión documental.
