![Sima2 Canary version](images/es-ES_simacanaryversionbn.png)   

Esta página contiene todas las **novedades** de **Ordering**.  
  
Haz clic en  [Subscribirme](http://eepurl.com/cZkO45) para recibir este **correo de novedades**.  
  
---    
  
# Versión 17.08.28  
  
**FUNCIONALIDADES GENERALES**  
  
 - Gestionar los distintos _source_ que envía Nadin.   
 - Procesar WE de _pesos_ y _emisiones_.   
  
**DETALLE DEL PEDIDO**  
  
 > **Notificaciones WLTP**  
 >> - Notificación en color rojo para los datos WLTP modificados durante los últimos 7 días.    
  
**MEJORA**  
  
 - **Ordering** muestra un mensaje avisando al usuario de que el catálogo de producto no está definido en su idioma.
   
---  

# Versión 17.08.14

**FUNCIONALIDADES GENERALES**    
  
 - Nueva página de **Subscribirme** para subscribirse o desuscribirse a la recepción del correo de nueva versión. También disponible desde la página de versiones. 
  
**DETALLE DEL VEHÍCULO** 

- Poder obtener y visualizar datos de WLTP que vengan de Nadin al hacer un chequeo a fábrica.
- Guardar los datos de WLTP obtenidos del chequeo a fábrica y guardarlos en el pedido.
- Actualizar los datos de WLTP enviados por la herramienta del Importador y asociarlos al pedido  correspondiente.  
  
**CESIONES**  

- Solicitar confirmación al aceptar o rechazar una solicitud de cesión.
- Poder aceptar cesiones de pedidos y transferir el pedido al nuevo concesionario.  
 - Realizar la cesion del pedido al aceptar la solicitud de cesión.  
 - No poder aceptar/rechazar solicitudes sobre pedidos en estado "No encontrado".  
  
---    

# Versión 17.07.28
  
 - Gestionar la comunicación con Nadin cuando existen peticiones pendientes de sincronizar
 - Enviar datos de entrega a Nadin al entregar vehículo
 - Poder recuperar un pedido del histórico bajo permisos específicos
 - Chequear una configuración antes de guardar un pedido cuando venimos de haber guardado un pedido previo y replicar la configuración.
 - El sistema envía a Nadin una asignación de cliente cuando por algún motivo esta haya desaparecido de Nadin.
 - Procesar la información de WLTP que nos pudiera venir de Nadin al hacer el order check para los distintos tipos de motorización.
 - Mejorar la gestión que se realiza cuando asignamos una fecha de venta sin fecha de llegada. De forma que no permite asignarla y da un mensaje a tal efecto.
 - Poder forzar que la fecha de entrega sea el dia en curso

---    
  
# Versión 17.06.21    
  
 - Controlar procesos de sincronización de información con el importador, evitando perder información no enviada previamente a la herramienta del importador (Nadin). 
 - Enviar a Nadin el cambio de visibilidad.  
 - Gestionar el permiso de recuperación de pedidos del histórico.    
  
---   
  
# Versión 17.06.20   
  
**FUNCIONALIDADES GENERALES**   
  
 - Eliminar un pedido, comunicándolo a Nadin, e indicando los errores de borrado según la respuesta del Importador (Nadin).   
 - Enviar datos de la matrícula al guardar los datos de entrega.   
  
**DETALLE DEL PEDIDO**   
  
 - Enviar una solicitud de borrado a Nadin en estados: _NewPending_ (0080), _Stored_ (0090), _ImpSec_ (0100), _Ordered_ (0200), _Order Cancelled_ (0275), _Frozen_ (0280) y _Scrapped_ (2700).        
 - Enviar a Nadin la asignación de cliente, vendedor, agente, tipo de venta.  
 - Poder modificar un pedido del que no tengo descripción. 
 - Enviar datos de matrícula al guardar datos de entrega.    
   
**CANCELACIONES**  
  
 - Visar notificaciones de cancelaciones pendientes de mis pedidos.  
  
**LLEGADA DE PEDIDOS**  
  
 - Mostrar en llegada de vehículos el dato de vendedor y del cliente.  
  
**GESTIÓN DE PERMISOS**  
  
 - Gestión de permisos para cancelaciones.     
  
**CORRECCIONES**  
  
**Corrección general**  
  
 - Se mostraba un error al cargar la página y la navegación https pasaba a http.  
  
**Detalle del pedido**  
  
 - No se mostraban los equipamientos en el detalle del pedido.  
   
  
---  
    
  
# Versión 17.05.24    
  
**NUEVAS FUNCIONALIDADES**     
  
  - Enviar datos de cliente (CD) a Nadin.  
  - Probar el envío de un Order Request solo con nº de pedido.  
  - Sincronizar con el importador un pedido no enviado a fábrica.  
  - Sincronizar un pedido en modificación pendiente o borrado pendiente.  
  - Enviar una solictud de borrado a Nadin.  
  - Enviar un pedido nuevo con un cliente nuevo.  
  - Avisar al usuario cuando un vehículo no tiene historial. 
  
**PANEL DE CONTROL**  
 
  - Poder hacer el envío de pedidos a Nadin desde la opción de menú y notificación _Pedido pendientes de envío_.    
  

  
**ENVÍO DE PEDIDOS**  
  
 - Enviar un pedido a Nadin.  
 - No enviar un pedido a fábrica directamente si tiene un error del fabricante.        
  - Enviar la modificación al importador.    
  - Modificar un pedido ya enviado.   
  - Probar el envío de un Order request sólo con nº de pedido     
  - Enviar un _NO_ y procesar la respuesta.   
  - Actualizar el pedido con el siguiente nº de pedido disponible ante error 18 en el envío de un _OE(N)_.     
  - Poder obtener el siguiente número de pedido disponible en Nadin.   
  - Modificar un pedido ya enviado.  
  - Enviar la modificación desde Ordering.  
  - Enviar un pedido nuevo con un cliente nuevo.     
   
**GESTIÓN DE USUARIOS**  
  
 > **Gestión de permisos**  
  
 >> - Gestionar en la edición de usuarios el permiso de envío de pedidos.      
  
  
**CORRECCIÓN**  
  
  - Se permite configurar modelos base cuando no existen versiones disponibles.      
  - Hacer el recorrido de compulsories completo teniendo en cuenta todas las combinaciones.   
  - Indicar que el vehículo seleccionado no tiene historial.

  
---  


 
# Versión 17.04.11   
  
  
**NUEVAS FUNCIONALIDADES**    
  
  > **Configurador**
  
 > - Se añade _Buscador de vehículos_ por código de equipamiento en los listados de pedidos.     
  
 > - Se lleva a una nueva versión el equipamiento existente en la versión previa aunque no esté disponible, en los siguientes casos:  
  >> - Descripción de familia no vigente.  
 >> - Descripción no vigente de equipamiento.  
 >> - Relación no vigente con modelo.  
 >> - No está relacionado o no existe definido para ese modelo.  
   
  
 > **Nuevo pedido**  
  
>  - Permitir múltiples equipamientos en la familia SNR.    
>  - Se añaden equipamiento en la versión aunque no muestren información de familia.  

  
 > **Pedidos pendientes de envió** 
  
>  - Enviar la confirmación de llegada al importador.      

    
  
**MEJORAS**     
  
 
 - Mejorar la forma de mostrar la información de los errores.  
  
**CORRECCIONES**   
  
 > **Editar pedido**     
  
 >>  - Recuperar el modelo en la edición de un pedido.    
  
 > **Nuevo pedido**        

 >> - Control de equipamientos eliminables de una versión al construir un pedido.  
  
 ---  

  
# Versión 17.03.17  
  
**NUEVAS FUNCIONALIDADES**    
  
 > **Detalle del vehículo**  
  
>> **Observaciones**
  
 >> - Poder editar observaciones, tanto  internas como externas. 
  
  
**MEJORAS**    

  - El texto del resumen de validación de pedido mejora su legibilidad y clarifica la información útil para el usuario.  
  
---  

  
  
# Versión 17.03.09    
  
**NUEVAS FUNCIONALIDADES**  
  
 - Poder consultar al Importador la información sobre un vehículo de nuestro concesionario.      
 - Procesar los errores de un pedido enviados desde el Importador.  
  
 >  **Detalle del vehículo**    
  
>>**Información de transporte**   
 
>> - Mostrar la información de transporte en el detalle del pedido y ​ asociada al vehículo ​​en cuestión.
  
>>**Observaciones**  
   
>> - Mostrar observaciones en el detalle del pedido, tanto internas como compartidas con el Importador.    
  
  
**MEJORAS**  
  
 - Proceso de comunicación con el importador.
  
  
**CORRECCIONES**  
  
 - La fecha de matrícula aparecía deshabilitada.  
 - Poder consultar el sistema del Importador, sólo vehículos propios activos y no entregados al cliente.



 
  
---  
   
  
# Versión 17.02.14   
  
**NUEVAS FUNCIONALIDADES**   
  
>   **Crear pedido**
  
 >> -  Comprobar el pedido con fábrica antes de guardarlo. Opción válida sólo para usuarios con permisos de acceso a fábrica.      
  
  > **Detalle del pedido**  
  
 >> -  Mostrar vehículos vendidos como demo asociados al clientes.  
 >> - Conocer el estado real y actual de un pedido, consultando con fábrica (Nadin) los últimos cambios del pedido.   
 >> - Recibir y procesar el OT recibido de Nadin.   
 >> - Procesar el OT recibido de Nadin.
  
 > **Listados de pedidos**
  
 >> - Poder consultar el estado de un pedido de mi concesionario que no esté en estado_Borrado_ ni _Modificación pendiente_.      
  >> - Contemplar los compulsories que puedan haber definidos en distintas filas para aquellos casos con más de 1 registro de compulsories.

  
**MEJORAS**  
  
 - Mejorar la interfaz del dashboard y menú de botones.   
 - Mejorar al solicitud de matrícula en Portugal.   
 - Mejorar traducciones de permisos.    
  


 
  
---  

 
  
# Versión  16.12.23  
  
**NUEVAS FUNCIOALIDADES**    
  
 > **Gestión de usuario**  
  
 >> - Chequear los permisos para confirmar las llegadas de pedidos al concesionario.  
 >> - Poder asignar/cambiar permisos para confirmar la llegada de vehículos al concesionario.  
 >> - Chequear permisos para bloquear pedidos.  
 >> - Poder asignar/cambiar permisos para bloquear pedidos.  
  
  
---  
   
  
# Versión 16.12.22    
  
**NUEVAS FUNCIONALIDADES**  
  

 > **Gestión de permisos**    
  
 > - Asignar/Cambiar permisos para modificar la configuración de un pedido (editar pedido).  
 > - Verificar permisos de usuario para Aceptar/Rechazar una solicitud de cesión de pedido de otro concesionario.  
 > - Asignar/Cambiar permisos para gestionar las solicitudes de cesión de pedidos (crearlas, aceptarlas, rechazarlas).  
 > - No poder eliminarme como usuario.    
  
 > **Gestión de matrículas**
    
 > - Solicitar matrícula (Portugal).  
 > - Las matrículas REQ no son tenidas en cuenta durante para dar de baja.  
  
 > **Configuración de pedidos**  
  
 > - Poder configurar un modelo base cuando no hay versiones.  
 > - Poder recuperar un modelo base cuando reconstruyo un pedido para modificar.    
  
 > **Gestión de cesiones**  

 > - Visualizar mensaje de cancelar solicitud de cesión.  
  
**MEJORA GENERAL**  
  
 > - Eliminar traducciones innecesarias.    
  
  
---  

  
# Versión 16.12.13      
  
**MEJORA GENERAL**  
  
 - Ubicación estándarizada para los botones Aceptar y Cancelar en ventanas modales.    

  
 **VEHÍCULOS DE OCASIÓN**     

 -  Acceder al detalle del cliente de un vehículo vendido como VO.
  
**GESTIÓN DE PERMISOS**  
  
 - Asignar permiso para modificar sólo pedidos propios o sólo cualquier pedido.    
- Controlar si tengo permisos para borrar pedidos.    
 - Chequear permisos al enviar una solicitud de cesión de pedido de otro concesionario.   
 - Asignar permisos para borrar sólo pedidos propios o cualquier pedido. 
   
 
**FICHA DE CLIENTE**
  
  - Mostrar campos obligatorios para  creación y edición del cliente.       
  
**GESTIÓN DE USUARIO**  
  
 - Mostrar campos obligatorios en la ficha del usuario.  
 - Mostrar campos obligatorios en el cambio de contraseña. 
  
**DETALLE DE PEDIDO**  

 - Bloquear la modificación de la matrícula y la fecha de matriculación de un vehículo.  
  
---  

  
# Versión 16.11.25    
    
**GESTIÓN DE USUARIOS**    
  
**Nuevas funcionalidades**
  
 - Verificar los permisos del usuario para crear pedidos y crear pedidos bloqueados.     
 - Asignar nuevo concesionario predeterminado a un usuario de mi concesionario.
 - Gestionar la creación de pedidos (bloqueados o no) según los permisos del usuario.
 - Informar al usuario de que no tiene permisos de creación de usuarios.
 - Editar permisos de creación de pedidos.  
  
**Correcciones**    
   
 - No se cargaban los equipamientos de modelo al seleccionarlo. 
  
  
--- 

 



  
# Versión 16.11.16  
  
**FUNCIONALIDAD GENERAL**
  
 - Unificación del nombre de empresas.  
 - Publicación del servicio web de imágenes.  
 - Buscar por descripción de versión de vehículo en el buscador general.  
  
**GESTIÓN DE USUARIOS**  
  
 - Asignar permisos de gestión de usuario a un usuario.  
  
**GESTIÓN DE DEMOS**  
  
 - Controlar y asignar la baja completa de un demo para entregar el vehículo.  
  
---  

      
  
# Versión 16.11.07 
  
**GESTIÓN DE USUARIO**  
  
 - Control de acceso a la gestión de usuarios.      
 - Eliminar los permisos de un usuario al eliminarlo dentro de un concesionario.  
  
**CONFIGURACIÓN DE VEHÍCULOS**  
  
 - No tener en cuenta las incompatibilidades entre paquetes (si tiene un mismo equipamiento) al realizar el pedido.   
  
---  


  
# Versión 16.11.04
  
**FUNCIONALIDAD GENERAL** 
  
  - Registrar ultimo login de acceso al concesionario al que accede un usuario.  
 - Mostrar logo de marca si no se encuentra imagen del vehículo en el fabricante.      

  
  
**MEJORA GENERAL**  
  
 - Se agrupan las distintas acciones de un listado en un botón único.  

  
**VEHÍCULOS DEMO**  
 
**Nueva funcionalidad**  
  
 - Asignar agente a un vehículo demo de mi concesionario.    
 - Asignar vendedor a un vehículo demo de mi concesionario.  
 - Asignar fecha de entrega a un vehículo demo.  
   
  
**GESTIÓN DE USUARIOS**  
  
**Nuevas funcionalidades**  
  
 - Modificar datos de usuarios de mi concesionario.   
 - Eliminar un usuario de mi concesionario.  
 - Marcar como _vendedor_ un usuario invitado en mi concesionario.       
      
     
  
**LOGIN**  
  
**Corrección**  
  
 - Se mejora el control del sistema cuando caduca la sesión del usuario de forma que no se muestra un error del sistema, sino el aviso de sesión caducada.
  

  


    
  
---  
    
  
# Versión   16.10.11

**MEJORA GENERAL**  
  
 - Formato para los campos obligatorios en los formularios (p.ej. Detalle de pedido).    
  
  
**CORRECCIÓN GENERAL**  
  
 - Cuando no hay combinación de equipamientos disponible aparecía un mensaje vacío.   

**GESTIÓN DE USUARIOS**    
>**Nuevas funcionalidades**  
   
> - Invitar a mi concesionario a otro usuario de otro dealer.      
> - Editar datos de un usuario de mi concesionario.
  
 
  
**VEHÍCULOS DEMO**  
  
>**Nuevas funcionalidades**    

  
> - Asignar fecha de venta.    
> - Editar un cliente asignado a un vehículo demo de mi concesionario.  


  
---  
   
  
  
  
# Versión 16.10.04    
  
  
  
**MEJORAS GENERALES**  
  
 - Mostrar logo de marca de vehículo si no existe imagen disponible del vehículo.  
 - Cerrar cesión para entrar con un usuario distinto al actual.   
    

**GESTIÓN DE USUARIO**    
  
>**Nuevas funcionalidades**

>- Crear nuevos usuarios para mi concesionario.  
 >- Visualizar los usuarios de mi concesionario.   
 >- Cambiar mi contraseña. 
  
**DETALLE DEL PEDIDO**    
  
>**Nuevas funcionalidades**  
  
 > -  Mostrar el TI y el DPW en el detalle del pedido.  
 > - Asignar fecha de entrega al cliente.  
 > - Poder asignar un tipo de venta desde el detalle de un pedido.   
 > - Aceptar una solicitud de cesión recibida.   
 > - Bloquear la modificación de visibilidad de un vehículo para los concesionarios.    
 > - Mostrar los campos obligatorios necesarios para entregar un pedido. 
 
>**Mejoras**    
  
 >- Se unificar botones de _Guardar_ en la sección de venta.   
   

  
**DETALLE DEL CLIENTE**  
  
>**Nuevas funcionalidades**  
  
 > - Definir el código postal del vehículo. 
   

**MODIFICAR VEHÍCULO**  
  
>**Nuevas funcionalidades**  
  
>- Identificar los equipamientos de versión no reconstruidos.    
>- Identificar los equipamientos de versión que no estén relacionados con el modelo.    
  
**VEHÍCULO DEMO**  
  
>**Nuevas funcionalidades**  
  
>- Buscar mis demos activos y pendientes de venta.  
  >- Asignar un cliente nuevo a un vehículo demo de mi concesionario.  
>- Asignar un cliente existente a un vehículo demo de mi concesionario.  
>- Quitar cliente asociado a un vehículos demo de mi concesionario.    

  
  
**VEHÍCULOS USADOS**   
  
>**Nuevas funcionalidades**  
  
> - Buscar mis demos no activos pendientes de venta.  


 
 
  
---  
 
  

# Versión 16.08.29 
  
**NUEVAS FUNCIONALIDADES**   
  
 - Recibir múltiples solicitudes de cesión sobre un mismo pedido.   
  
   

**Gestión de clientes**  
> - Menú para la gestión de clientes de mi concesionario.  
> - Buscar clientes de mi concesionario.  
> - Visualizar los pedidos asociados de un clientes.   
> - Mostrar los vehículos que tienen los clientes de mi concesionario (pedidos activos asociados y en el histórico).

  
 **Detalle del pedido**   
> - Marcar clientes como _deshabilitados_ para evitar asociarlos a pedidos. 
> - Asignar vendedor.
> - Visualizar los errores de fábrica con su código y descripción en el detalle del pedido.   
> - Visualizar los equipamientos y sus descripciones agrupados por tipo de equipamiento (versión, opcionales, serie). 
> - Acceder al detalle del pedido desde pedidos _con modelo no disponibles_.  
> - Acceder al detalle desde solicitudes de cesión enviadas.   
> - Mostrar los equipamientos agrupados y sus descripciones (botón _ver más_).  
> - Asignar vendedor desde el detalle de un pedido propio.  
   

 - **Historial del pedido**    
  
> - Visualización del historial de cambios del pedido. 

  
 - **Modificación de pedidos**

>- Se aplican las reglas de catálogo para pedidos en estado _Guardado Desy_ al modificar los pedidos, excepto en los casos de modificaciones de _equipamientos  de versión no relacionados con el modelo_ y _equipamientos de versión no vigentes para el modelo asociado_. Será añadidos en próximos despliegues.
  

 -  **Configurador de pedido**  
   
> - Visualizar la configuración previa del vehículo durante la modificación de su pedido.
 
  
**MEJORAS**    
    
 - El combo de selección de concesionarios los muestra en orden cronológico.   
 - Visualizar el código de concesionario e información adicional (tooltip) en el listado de pedidos de red.    
 - Mostrar solamente las solicitudes recibidas en estado pendiente.   
 - Controlar la modificación y borrado de fechas.   
  
  
---
#Versión 16.07.08  
  
**NUEVAS FUNCIONALIDADES** 
  
 - Borrar pedidos, individual o masivamente, en estado _Not found_, _Deleted_ y _Order cancelled_.
 - Ver mis solicitudes de cesiones enviadas.  
 - Poder solicitar una cesión da un pedido visible de otro concesionario.  
 - Mostrar en el detalle de un pedido propio si su cesión ha sido solicitada.    
  Poder rechazar una solicitud de otro concesionario sobre un pedido propio.  
 - Poder cancelar una solicitud de pedido de red.  
  - No tener en cuenta las solicitudes de cesión canceladas ni aceptadas para poder volver a solicitar una cesión.    
 - Poder filtrar por estado las solicitudes enviadas.  
 - Ver solicitudes rechazadas.  
 - Poder editar un cliente desde el detalle de un pedido.  
 - No se muestran los pedidos de red en error o aviso si soy un concesionario.   
 - Se impida la creación de nuevos clientes cuando el pedido es de stock. 
  
---  
 
 
#Versión 16.06.17

**NUEVAS FUNCIONALIDADES** 

- Controlar máscaras de matrículas: el sistema evaluará las máscaras de matrícula activas en el sistema. De momento las matrículas deberán ponerse en mayúsculas, tal y como esté el criterio de máscara de matrícula.
- Poder editar el cliente asignado a un pedido desde el detalle del pedido. Esto incluye la modificación y su encolado para la comunicación con el sistema del importador (Nadin para el caso del grupo VW).

**MEJORAS**  

 - Bloquear el botón de nuevo cliente en la creación de un pedido cuando indicamos que el pedido es de stock.
 - Se mejora el proceso de despliegue de la aplicación para que se apliquen los cambios de autenticación integrada con el dominio. 
 - Se mejora la apariencia del detalle de un pedido en bloques bien diferenciados.
 - Ajustar los colores de la zona de notificaciones del Dashboard para que se muestren de una forma más legible.

---    


#Versión 16.06.09  



**NUEVAS FUNCIONALIDADES**  
   
 -   Mostramos en el dashboard un informe de los pedidos en stock por grupo modelo, pudiendo desmarcar algunos grupos modelos y trabajar dinámicamente sobre los mismos. 
 -   Bloquear cambios en los casos que un vehículo, por su estado no lo permita.
 -   Poder asignar matrícula y fecha de matrícula a un vehículo. 
 -   Establecer fecha de venta para un vehículo.
 -   Poder hacer búsquedas en el histórico de pedidos.
 -   Poder acceder al detalle de un pedido que está en el histórico.
 -   Si no encuentro un vehículo en el activo, poder buscarlo en el histórico y viceversa.
  
**MEJORAS**  

 - Controlamos el no poder configurar modelos base si la marca lo tiene así definido.
 - Ajustar el detalle de un pedido de forma que quede más homogénea.

---  
#Versión 16.05.17  


**NUEVAS FUNCIONALIDADES**  

 -   No poder usar un modelo base para una configuración para los concesionarios definidos.   
 -   Poder seleccionar el tipo de venta al configurar el pedido.   
 -   Se muestra el tipo de error en la página de **Pedidos con error**. 
 -   Incluir el código del timing-indicator (semana de producción) en el **Configurador**.  
 -  Incluir los códigos de modelgroup y modelo en el **Configurador**.  
 -  Se muestran los errores de NADIN en la página de **Pedidos con error** en el idioma seleccionado por el usuario.
  
**MEJORAS**  

 - Las notificaciones se ordenan según su criticidad y se ocultan aquellas notificaciones a 0.

---  

#Versión 16.05.05  

 

**NUEVAS FUNCIONALIDADES**  
  
  
- Acceder al detalle de un pedido. Se identifica  el tipo de pedido (cliente de red o propio) y su visibilidad.
- Crear un nuevo cliente y asociarlo a un pedido. Se realiza un chequeo de duplicidad de cliente.  
- Cambiar la asignación de un cliente a un pedido, sin tener que quitar al cliente y volver  ponerlo y evitando cambios de visibilidad.  
>- Permite mantener la fecha de contrato original.  

- Quitar la asignación de un cliente a un pedido.  
- Cambiar la visibilidad de un pedido.
- Asignar la visibilidad a un pedido después de quitarle el cliente.
- Ajustar los formatos de fecha de acuerdo a la configuración del cliente.  
- Control de clientes potencialmente duplicados. Se incluye la información de los clientes que pueden estar duplicados para poder valorar si se trata realmente de dicho caso. 
  
**MEJORAS**  
  
 - Se muestra la imagen del vehículo en la página de **Nuevo pedido**. 

  


  

 


  





  
   



