# PROYECTOING2

## Requerimientos no funcionales (RNF)
1. **Rendimiento**
   - El sistema debe responder en menos de X segundos para operaciones comunes (p. ej., búsqueda y carga de listados).
   - El tiempo de carga de pantallas principales no debe exceder X segundos con carga normal.

2. **Disponibilidad**
   - El sistema debe mantener disponibilidad objetivo de **99.5%** (ajustable según tu necesidad) mensual.
   - Debe existir manejo de fallos (reintentos y mensajes claros).

3. **Seguridad**
   - Las contraseñas deben almacenarse con hash seguro.
   - El sistema debe usar HTTPS.
   - Debe aplicar control de acceso basado en roles/permisos para todas las rutas y acciones.
   - Debe prevenir inyección SQL/XSS usando validación y codificación segura.

4. **Integridad y consistencia**
   - El sistema debe garantizar consistencia de datos en operaciones transaccionales.
   - Debe validar reglas de negocio antes de guardar cambios.

5. **Usabilidad**
   - La interfaz debe ser navegable y consistente.
   - Debe permitir recuperar el usuario de errores comunes con mensajes comprensibles.

6. **Mantenibilidad**
   - El sistema debe estar estructurado para facilitar mantenimiento (módulos claros, estándares de código).
   - Debe incluir documentación mínima (arquitectura, despliegue y APIs si aplica).

7. **Escalabilidad**
   - Debe soportar aumento progresivo de usuarios y carga de trabajo sin degradación significativa (según objetivo).
   - Debe permitir escalar componentes (aplicación y/o base de datos) si aplica.

8. **Compatibilidad**
   - El sistema debe funcionar en navegadores modernos (p. ej., Chrome, Edge, Firefox, Safari).
   - Debe ser responsive para móvil/tablet si aplica.

9. **Compatibilidad e interoperabilidad (si aplica)**
   - El sistema debe integrarse con servicios externos mediante API (si aplica).
   - Debe manejar formatos de intercambio definidos (JSON/XML) y versionado si aplica.

10. **Observabilidad**
   - El sistema debe registrar logs de aplicación y errores.
   - Debe proporcionar métricas básicas (latencia, errores) y trazabilidad para depuración.

11. **Respaldo y recuperación**
   - Debe realizar copias de seguridad programadas de la base de datos.
   - Debe permitir recuperación en un tiempo objetivo (RTO) y con datos acordes (RPO).

## Requerimientos funcionales (RF)
1. **Autenticación de usuario**
   - El sistema debe permitir registro, inicio de sesión y cierre de sesión.
   - El sistema debe validar credenciales y manejar sesiones.

2. **Gestión de usuarios**
   - El sistema debe permitir visualizar el perfil del usuario.
   - El sistema debe permitir editar datos permitidos (p. ej., nombre, correo, contraseña).

3. **Roles y permisos**
   - El sistema debe soportar al menos dos roles (p. ej., usuario y administrador).
   - El sistema debe restringir acciones según rol.

4. **Gestión de entidades principales (según tu caso)**
   - El sistema debe permitir crear, editar, listar y eliminar registros de la(s) entidad(es) definida(s) (p. ej., productos, solicitudes, documentos, tareas).
   - El sistema debe permitir búsqueda y filtrado por campos clave.

5. **Flujos del negocio**
   - El sistema debe permitir ejecutar el proceso principal (p. ej., crear una solicitud, asignarla, aprobarla/rechazarla, cerrarla).
   - El sistema debe guardar el estado de cada proceso y permitir transiciones válidas.

6. **Notificaciones**
   - El sistema debe mostrar notificaciones en pantalla (p. ej., confirmaciones, errores).
   - El sistema debe enviar notificaciones (si aplica) por email o similar cuando ocurra un evento relevante.

7. **Auditoría (trazabilidad)**
   - El sistema debe registrar acciones críticas (creación, modificación, borrado, aprobación).
   - El sistema debe permitir consultar el historial de cambios de un registro.

8. **Reportes y exportación**
   - El sistema debe generar reportes básicos (por rangos de fechas, filtros, estados).
   - El sistema debe permitir exportar reportes a un formato (p. ej., CSV/PDF) si aplica.
