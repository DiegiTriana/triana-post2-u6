# U6 Post-Contenido 2 - Spaghetti Code a Strategy + Command

## Objetivo
Eliminar Spaghetti Code de procesamiento de pedidos aplicando:
- Patron Strategy para reglas de descuento.
- Patron Command para desacoplar solicitud y ejecucion.

## Estructura clave
- `ProcesadorPedidos`: version inicial con condicionales anidados (conservada).
- `EstrategiaDescuento` + `DescuentoVIP`, `DescuentoPremium`, `DescuentoEstandar`.
- `ComandoPedido` + `ComandoProcesarPedido`.
- `SelectorEstrategia`.
- `Main` con flujo refactorizado.

## Ejecutar
```bash
mvn clean compile
mvn exec:java
```

## Resultado esperado
El flujo final mantiene los casos de negocio, reduce anidamiento y mejora testabilidad al separar decisiones y acciones.
