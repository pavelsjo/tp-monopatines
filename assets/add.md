# 1. ITERACION

- [Buena latencia](https://clients.amazonworkspaces.com/Health.html) (probada). Nos conectamos y dio una velocidad de 37 mseg de Round Robin.
- Conocimientos técnicos en el sector que facilitan la implementación
- En abril del 2022 anunciaron a futuro instalacion de DCs en Buenos Aires
- Brinda escalabilidad y disponibilidad
- Servicio Near real-time: comunicacion mediante Kafka (Amazon MSK) y API Gateway (microservicio) para página web
- AWS MSK no orquesta los servicios por si solo (necesita un orquestador intermediario)
- No hay limitaciones que obligan a usar DCs on-premise

# 2. ITERACION 

QA de seguridad, gestión de usuarios
- AWS Amplify Feature: Authentication
- Permite loguearse mediante uso de Social Networks
- Puede agregar autenticacion con doble paso
- Permite configurar el inicio de sesion
- Ya almacena a los usuarios, sin tener que crear una DB desde cero, y se les puede agregar permisos (útil para administrativos)
- Se puede usar librerias para agregar funcionalidades extras a la autenticacion (el SHA512)
https://aws.amazon.com/amplify/authentication/

# 3. ITERACION 
Pago de servicio con MELI
-API de MercadoPago (Microservicio) que se encargue de conectar MercadoPago, y solicitar el saldo
-RDBMS en donde se almacena la información del saldo de los usuarios: Amazon RDS
https://www.mercadopago.com.ar/developers/es/reference
https://aws.amazon.com/es/getting-started/hands-on/create-mysql-db/

# 4. ITERACION 

Una única DB que tenga toda la información asociada al estado de los monopatines (con o sin mantenimiento). Esto facilita la sincronización de datos entre DBs replicadas

# 5. ITERACION 

Se utilizó HAIKU como estrategia de documentación por que era un método simple y rápido que incluia los objetivos de negocio.