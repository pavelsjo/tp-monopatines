# Diseño de Arquitectura para Sistema de Monopatines Eléctricos

Identificar los principales `requerimientos funcionales` y de `calidad (no funcionales)` del sistema.

### Requerimientos Funcionales

- Generar reporte de uso de monopatines por:
    - Kilómetros.
    - Tiempo con pausas.
    - Tiempo sin pausas.

- Registrar 
    - Monopatín en mantenimiento.
    - Fin de mantenimiento de monopatín.

- Administrar
    - Ubicar monopatín en parada (opcional).
    - Agregar monopatín.
    - Quitar monopatín.
    - Registrar parada.
    - Quitar parada.
    - Definir precio.
    - Registro de usuario.
    
- Definir tarifa extra para reinicio por pausa extensa
- Anular cuenta.
- Cargar dinero.
- Descontar dinero.
- Activar monopatín
- Pausar monopatín/viaje.
- Empezar viaje.
- Terminar viaje.
- Quitar pausa monopatín.
- Generacion de url para codigo QR.
- Identificar monopatín por código QR.

### Requerimientos No Funcionales

- El sistema debe estar disponible el 99% del año 
- El sistema debe tener una ventana de mantenimiento de 1 día al año.
- El sistema deberá soportar un máximo de 100.000 usuarios logueados y utilizando la aplicación al mismo tiempo.
- El sistema deberá encriptar los datos personales de los usuarios almacenados en la base de datos.
- El sistema deberá proveer una interfaz WEB responsive.
- El sistema no deberá de tardar más de 5 segundos en cargar el listado de cuentas de MELI Asociadas.
- El tiempo de respuesta del sistema a peticiones de usuarios no debe superar los 10 segundos en **todas** las interacciones con la app. Ejemplo: Pagar, Solicitar, Cancelar, Pausar y Finalizar.

### Restricciones

-  La aplicación móvil para los usuarios del servicio
-  Debe contar con una aplicación Web para la gestión correspondiente.

## Stakeholders

- Usuario final.
- El dueño de la aplicación.
- Departamento de Sistemas.
- Administradores.
- Proveedores de Monopatines.
- Los que hacen mantenimiento.
- Autoridades del Gobierno local.

## User Stories

- Crear una nueva cuenta:
    - Como usuario final necesito crear una nueva cuenta en la aplicación para poder utilizar el servicio.
- Asociar cuenta mercado pago:
    - Como usuario final necesito asociar una cuenta de mercado pago previamente creada y asociarlo con mi cuenta de la aplicación para poder tener créditos.
- Iniciar viaje:
    - Cómo usuario final necesito una interfaz intuitiva para ubicar la parada más cercana con monopatines disponibles, abonar el pago y usar el monopatín.
- Administración de aplicación:
    - Como administrador necesito agregar, pausar eliminar las paradas ylos monopatines.
- Mantenimiento de monopatines:
    - Como usuario de mantenimiento necesito saber el tiempo de uso y los kilómetros recorridos de cada monopatín para determinar si es requerido un mantenimiento.

## Requerimientos de calidad & Vinculación

- Performance.
    - Usuario final.
    - Administradores
- Escalabilidad.
    - El dueño de la aplicación.
    - Administradores
- Disponibilidad.
    - Usuario final.
    - El dueño de la aplicación.
- Seguridad.
    - Usuario final.

## Utility tree.

![img](https://raw.githubusercontent.com/pavelsjo/tp-monopatines/main/assets/img/utility-tree.jpeg)

- Lenyenda
    - (Importancia, Complejidad).
        - High - (H).
        - Medium - (M).
        - Low - (L).
