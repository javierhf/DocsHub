![sima2](images/es-ES_simacanaryversionbn.png)  
   
 
Esta página contiene todas las **novedades** de **SIMA Service**.        
  
---    
# Versión 17.08.29  
  
**ESTADO DE CARRILES**  
  
 - Eliminar de los carriles los vehículos con citas canceladas o pospuestas.  
  
**CORRECCIONES**  
  
 > **Crear cita**  
  
 > - Se muestra, actualizado, el panel de disponibilidad de horas del asesor tras hacer clic en _Crear_.
  
  
---  
 
# Versión 17.08.02
   
**NUEVAS FUNCIONALIDADES**    

- Incluir letras motor en la información del vehículo en la oportunidad y durante la cita. 

>**CITA**

> - Poder añadir trabajos de concesionario con servicios externos y otros cargos. 

**MEJORAS**

>**LOGÍSTICO**

> - Sólo aparezcan para retirar vehículos que han entrado con renococimiento de matrícula. 
> - El listado de vehículos a retirar se refresque cuando se visualiza la pantalla, tras el desbloqueo del móvil, cambio de pestaña en el navegador.
> - Se comunique en tiempo real a otros logísticos que un vehículo ya fue retirado por un logístico. 
> - Aparezcan todos los vehículos pendientes de retirar de los carriles o el parking, independientemente del estado de la orden y de la fecha de llegada.
> - Añadir ubicación y fecha de recepción en los coches pendientes de retirar, resaltando en color los de días anteriores. 

>**ESTADO DE CARRILES**

> - Cambio icono papelera por tick, para evitar dudas en los usuarios. 
> - Añadir ubicación y fecha de llegada, resaltando en color los de días anteriores. 

 --- 

# Versión 17.07.24   
  
**NUEVAS FUNCIONALIDADES**    

> **CLIENTE**

> - Visualizar el domicilio del cliente durante la cita.
> - Modificar las observaciones del cliente en cita y ficha oportunidad. 
  
> **VEHÍCULOS SUSTITUTIVOS**

> - Seguimiento de reservas de vehículos sustituvos. 
> - Entrega de vehículos, con firma digitalizada y envío de correo con el contrato firmado al cliente. 
> - Posibilidad de diseñar un layout específico para el email que se envía con el contrato adjunto.  
> - Nuevo layout para definir las condiciones generales del contrato, usado para mostrarlo en la web y en el contrato que se envía al cliente.
  
> **GESTOR DE CLIENTES**    

> - Mostrar información del vehículo sustitutivo reservado al recepcionista.    
> - Descartar un vehículo sin cita.
  
> **GESTIÓN DE CITAS DEL PORTAL DE CLIENTE**    

> - Visualizar el listado de citas creadas desde el portal de cliente.  
 
**MEJORAS**     

> - Cambio componente de la agenda asesores en la cita para poder visualizar huecos libre y ocupados, facilitando averiguar la carga. 

**CORRECIONES**     

> - Se corrigen errores relacionados con zonas horarias, que hacían que no se mostrara la disponibilidad o se mostrara de forma incorrecta en la agenda de los asesores durante la cita.
> - Mejora de los logs internos de las operaciones del logístico.
> - Usuarios con puesto general no se muestren en la agenda como disponibles.

---  

# Versión 17.06.14   
  
**CORRECCIONES**    
  
> - Al buscar trabajos por talleres se buscaban en todos los talleres. Ahora se mostrarán sólo los trabajaos del taller al cual se añadirán.

 ---  
  
# Versión 17.04.18   
  
**NUEVAS FUNCIONALIDADES**    
  
> **Creación de la cita**
  
 > - Permiso de gestión para los vehículos sustitutivos, tanto en el  mantenimiento de Movilidad como en el Tarifario y Vehículos de sustitución.  
 > - Venta activa marca Ducati.  
 > - El cambio de configuración no sobreescribirá el fichero del target  con el siguiente despliegue. Si no existe el fichero de configuración, se aplicará el fichero definido por deceto.    
  
**CORRECCIONES**  
  
> **Creación de la cita**    
  
> - **Reserva de hora para asesores:**   
 >> - No se estaba trabajando con hora UTC y la disponibilidad de los asesores se mostraba desplazada, según la diferencia horaria respecto al UTC.      
 >> - Se comprueba que la hora de la cita creada corresponde con la indicada en la _Creación de la cita_.      
 
---     
  
# Versión 17.04.11     
  
**NUEVAS FUNCIONALIDADES**  
  
 > **Creación de la cita**  
  
> - Añadir observaciones al trabajo.   
> - Añadir observaciones a la orden.    
  
> **Vehículo sustitutivo**  
 
> - Mostrar el número de orden en el formulario de reserva de vehículo sustitutivo.  
  
---  
  
# Versión 17.03.13      
  
**NUEVAS FUNCIONALIDADES**

 > **Ficha de cliente**  
  
 > - Visualizar las ofertas de PPSO y Active Selling.  
 > - Visualizar nombre de último depositario.    
   
 > **Cita de taller**  
    
 > - Visualizar campañas de ElsaR durante la creación de la cita.  
  

  
 > **Paquetes PPSO**
  
 > - Visualizar el detalle de un paquete de PPSO en la ficha de cliente.     
  
 > **Añadir trabajos**   
  
 > - Añadir trabajos sin posiciones  definidas.
  
 > **Permisos de usuario**  
  
 > - Bloquear creación de citas para usuario que no tengan los permisos adecuados.  
 
---  

  
# Versión 17.01.26  
  
**NUEVAS FUNCIONALIDADES**     
  
 > **Gestor de clientes**
    
 > - Buscador de clientes por _tercero_ y _matrícula_.    

---  

  
# Versión 17.01.23      
  
**NUEVAS FUNCIONALIDADES**  
  
> **Gestor de clientes**      
  
> - Notificar que ha llegado un cliente sin cita.     
  
> **Logístico**  
  
> - Visualizar los coches en espera para entrar en el taller (ya recepcionados).   
> -  Visualizar que ya se ha retirado un coche para tener sólo coches pendientes de retirar.    
  
**MEJORAS**  
  
 > - Mostrar los precios según moneda definida para la empresa.    
 > - Mostrar kilómetros del vehículo en el histórico de reparaciones.
  
---  
   
# Versión 16.12.22      
  
**NUEVAS FUNCIONALIDADES**  
  
 > **Tarifario**  
  
> - Dar precio a vehículos sustitutivos de alquiler.  
> - Gestionar grupo y tarifa de vehículos sustitutivos.  
  
> **Creación de la cita**  
  
> - Mostrar precios de los vehículos sustitutivos cuando son de alquiler.    
  
> **Gestor de clientes**  
  
> - Mostrar aviso cuando ha llegado un cliente sin cita.
  
**MEJORAS**    

 > - Se añade texto "El cliente dice que..." en trabajos libres.  
    
---  
  
# Versión 16.11.21    
  
**NUEVAS FUNCIONALIDADES**
  
 
 > **Gestor de clientes** 
  
 >> - Visualizar para el recepcionista que el cliente llegó.  
 >> - Visualizar para el recepcionista que el vehículo ya se está recepcionando.  
 >> - Comunicar a otro usuario en el gestor de clientes que un cliente llegó.
  
> **Active Search**  
  
 >> - Mostrar campañas de mercado pendientes de realizar o planificar.  
  
 > **Creación de la cita**  
  
**CORRECCIONES**    
  
 > - No se podía crear cita si el campo observaciones es muy grande en el seguimiento de la orden.     
  
 > - No se visualizaba la reserva creada sobre un vehículo sustitutivo durante la creación de la cita.

---       
   
# Versión 16.31.10     
 
  
**MEJORA GENERAL**  
  
 > - Mejora del rendimiento en el cálculo del target de siguientes mantenimientos.   
  
---  
  
# Versión 16.10.05 
  
**NUEVAS FUNCIONALIDADES**    
  
> **Ficha de cliente**    
  
> - Consultar toda la información de contacto de un cliente.   
> - Editar el medio de contacto de un cliente. 
> - Indicar cómo quiere ser contactado el cliente para recordarle la cita. 
  
> **Creación de la cita**    
  
> - Crear cita para vehículo borrador.     
> - Envío de correo electrónico de confirmación de cita al cliente.  
> - Plantillas personalizadas por marca para el correo electrónico recordatorio de cita.      
  
**MEJORAS**    
  
> **Creación de la cita**  
  
> - Cambio de nombre del botón _Guardar_ por _Crear_ para aclarar el comienzo y fin del proceso de creación de la cita.  
> - Ajuste automático de las siguientes citas disponibles cuando se modifica la duración de una cita anterior.
    
**CORRECCIÓN**  
  
 > - Al crear una cita se producía un error cuando no se tenía letras de motor.  

---  
  
# Versión 16.09.26    
  
**NUEVAS FUNCIONALIDADES**  
  
 > - Buscador de vehículos admite búsquedas mediante nombre de cliente.    
 > - Acceso a los avisos asociados a un cliente desde la ficha de cliente..

**CORRECCIONES**  
  
 > - Agregar idioma al componente _remoteselect2_.
  
**GESTOR DE CLIENTES**  
  
> **Nuevas funcionalidades**  
   
 >> - Visualizar la solicitud de taxi hecha por el cliente.    
 >> - Visualizar la solicitud de recepción activa para un cliente.  
  
**CREACIÓN DE LA CITA**   
  
 > **Nuevas funcionalidades** 
  
  >> - Indicar que el cliente solicita taxi.    
  >> - Indicar que el cliente acepta recepción activa.  
  
 > **Mejoras**  
  
 >> - Nuevo diseño del resumen de cita para mejorar la lectura de la información. 
  
---  
  
# Versión 16.09.07    
  
**CREACIÓN DE LA CITA**  
  
 > **Nuevas funcionalidades**  
>  
 > - Sólo se muestran las campañas de las que es responsable mi concesionario.     
  
 > **Mejoras**
  
 >> - Crear averías con texto de una máximo de 100 caracteres.  
 >> - Eliminar paquetes de importador en el concesionario después de añadirlo (Market packages).  
 >> - Acotar visualmente el tamaño del nombre de los clientes. 
  
**MEJORAS**   
 
> - Hacer que el tooltip funcione en todos los exploradores.   
  
---  
  
# Versión 16.09.02  
  
**GESTOR DE CLIENTES**      
  
>**Nuevas funcionalidades**  

> - Indicar qué vehículo ha llegado para su cita en el taller.  
> - Consultar vehículos de próximas citas del día.     
    
**CREACIÓN DE LA CITA**      
  
>**Nuevas funcionlidades**
  
  >  - Editar el tiempo estimado inicialmente para un trabajo.  
  >  - Duración segmentada para los trabajos.  

>**Mejoras**    
  
 >>**Vehículos bajo campañas**
  
   >>>  - Los filtros de campañas aplicados se mantienen durante la navegación hacia delante y hacia atrás.  

---  

   
  
  
# Versión 16.08.16   
  
**NUEVAS FUNCIONALIDADES**     
  
 - **Campañas**   
> - Añadir campañas aplicables al vehículo durante la creación de la cita.
    
  
  
**MEJORAS**  
  
- **Oportunidades** 
> - Los vehículos vendidos por nuestros agentes no se muestran como oportunidades.

---    


# Versión 16.08.10   
  
**NUEVAS FUNCIONALIDADES**     
  
 - **Campañas**  
  
> - Seleccionar marca y campañas para visualizar vehículos (VIN) afectados.  
> - Añadir campañas aplicables al vehículo durante la creación de la cita.

    
 - **Paquetes**    
 
> - Visualizar y añadir los paquetes del Importador y el Concesionario para dar precio al cliente.      
  
  
**MEJORAS**  
  
- **Oportunidades**  
> - Los vehículos vendidos por nuestros agentes no se muestran como oportunidades.     

- **Paquetes**  
> - Se visualizarán los paquetes del vehículo según marca, independientemente de que el VIN del vehículo exista en el Importador.      
  
 - **Medio de contacto**  
 
> - El medio de contacto  por defecto con el cliente queda indicado según los medios de contacto activos para el mercado.   
 
---    
# Versión 16.07.21  
  
 **NUEVAS FUNCIONALIDADES**  
  
  - Añadir paquetes/ofertas de cualquiera marca durante la creación de la cita.  
 - Añadir paquetes del propio concesionario durante la creación de la cita.  
  

**MEJORAS**  

  - Se amplia a más de 15 días la fecha para la cual se puede dar cita al cliente.   

---      
  
# Versión 16.07.08  

**NUEVAS FUNCIONALIDADES**  

 - Indicar que una avería es repetitiva en el proceso de creación del a cita.  
  
---  
   
  
# Versión 16.06.29  
  

**NUEVAS FUNCIONALIDADES**  

         
 - Crear cita para cualquiera de los talleres de la empresa.  
 - Histórico de reparaciones accesible desde las fichas de Active Search y la Creación de Cita.  
  
---  

#Versión 16.05.05  

**NUEVAS FUNCIONALIDADES**  

  - Consultar las campañas ya realizadas.  
  
**MEJORAS**  

 - Información de comunicaciones ampliada.   
 - Búsqueda mejorada de vehículos por matrícula.    
 
---  
# Versión 16.03.23   

**NUEVAS FUNCIONALIDADES**    
  
  - Selector de cambio de empresa.
 
**MEJORAS**  

 - Se limita el abrir nuevas pestañas por cada acción de usuario.   
 - Selector de cambio de empresa.

**MEJORAS**  

 - Se limita el abrir nuevas pestañas por cada acción de usuario.  
   
**CORRECCIONES**  
  
 - Se desvincula sistema de recordatorios a través de Exchange.

---  

# Versión 16.03.07 

**NUEVAS FUNCIONALIDADES**   
 
- Listado de vehículos afectados por campañas.    
- Recoger feedback de una campaña ofrecida.    
- Indicar que un mantenimiento ya ha sido planificado para evitar ofrecérselo de nuevo al cliente.  



---  
# Versión 16.02.23  

**NUEVAS FUNCIONALIDADES**   

 - La ficha de oportunidad muestra ahora los _precisas_ recogidas desde Mobile Workshop.  
 - El target de _Precisas_ solamente muestra aquellos precisa pendientes.  
 - Se muestra un Panel con aviso para recordatorios de oportunidades para hoy.  
    

**MEJORAS**  
 
 - Solamente se pueden introducir observaciones si se ha seleccionado un feedback.  
   
---    

# Versión 16.02.11  

**NUEVAS FUNCIONALIDADES**   
 
 - Aplicar distintas configuraciones según mercado y marca de trabajo del usuario.
 - Lista de Precisa (Mobile Workshop) en el menú de la derecha.

**MEJORAS**  
    
 - El target de bujía solamente aplica a vehículos de gasolina.  
 - La configuración del servicio de mantenimiento es distinta según las letras de motor.  

---     
 

# Versión 16.01.25  
   
 
**NUEVAS FUNCIONALIDADES**    

 - Target de llamada de Vencimiento de garantía.  
 - Target de bujías incluye configuración por letras letras de motor.     
 - Feedback para varios mantenimientos a la vez y de una llamada entrante del cliente.  
 - Acceso a empresas de Opportunity en distintos entornos.
     
**MEJORA**  
  
 - No se incluyen los vehículos con cadenas en Target de correas.    
 - Actualizar la fecha de próximos mantenimientos según el feedback de km dados por el cliente.
 - Nuevo motivo de rechazo "Lo realizará en otro servicio oficial".

---  

# Versión 16.11.01  

 **NUEVAS FUNCIONALIDADES**    
 
 - Acceso a listado de oportunidades con feedback de Recordatorio.  
 - Target de llamada para líquido de frenos.   
 - Tabulación del feedback para motivos de rechazo. 
 
 **MEJORAS**  

  - El recordatorio en Outlook no estaba indicando a qué concesionario pertenece la oportunidad.  
    
---  

# Versión 15.12.18  

**NUEVAS FUNCIONALIDADES**  

 - Target of call for next timing-belt change.  
 - Target of call for spark-plug change.  
   
**MEJORAS**      
   
 - La ficha del cliente muestra información sobre la _Última inspección_ y la _Fecha estimada_ del plan de mantenimiento.  
 
---  

# Versión 15.12.02     
**NUEVAS FUNCIONALIDADES**    

 - Navegar por las oportunidades. 
 - El feedback _Llamar en otro momento_ aparece de nuevo como nueva oportunidad en el target.  
- Abrir oportunidades desde el buscador de matrículas.  
- Target para _Siguientes mantenimientos_. 
  
---

# Versión 15.11.20  
  
**NUEVAS FUNCIONALIDADES**    

 - Añadidos a oportunidades los vehículos que pertenecen a flotas cuando el depositario no es flota ni concesionario. 
 - Acceso a la Ayuda de usuario.
   
  
**MEJORAS**  
  
 - Mejorar la interfaz y experiencia del usuario.  
   
---  
  
# Versión 15.11.04  
**NUEVAS FUNCIONALIDADES**    
 
- Chequear automático los clientes con contrato de mantenimiento o extensión de garantía.  
- Registro para llamar en fecha dada.  
- Control visual del número total de oportunidades.    
- Se muestran las campañas del fabricante.  
- Se muestran los kilómetros y estimación de kilómetros y primer mantenimiento.  
- Feedback para los kilómetros de los que informa el cliente.  
- Control de la frecuencia de llamadas para clientes que no contestan.  
- Mostrar solamente marcas relacionadas con el primer mantenimiento.  

**MEJORAS**    

 - La estimación desecha el kilometraje tomado durante el primer mes del vehículo.   

---  

# Versión 15.10.27  
**NUEVAS FUNCIONALIDADES**   
 
- Feedback para _Llamar en otro momento_.
- Nuevo tiempo de 22 meses para entrar en Opportunity. 
- Mostrar VIN del vehículo.  

---  
 
# Versión 15.10.07  
**NUEVAS FUNCIONALIDADES**   
 
- Mostrar el propietario del vehículo.  
- Contactar por correo con el cliente para primer mantenimiento.
- Mostrar información de las garantías.
- Priorizar las _Oportunidades_.  

**MEJORAS**  
  
- No se proponen clientes de rent-a-car.
- No se proponen clientes de vehículos de traspaso entre concesionarios.   
 
---  

# Versión 15.09.11    

**NUEVAS FUNCIONALIDADES**  
 
-  _Target_ para clientes que deben ser contactados por teléfono.  
- Histórico de contactos ya realizados con un cliente.    
- Interfaz para registrar recordatorio y feedback positivo y negativo.
