![sima2](images/es-ES_simacanaryversionbn.png)  
  
---    
  
# Target

**Target** es el conjunto de fichas cliente/vehículo u _oportunidades_ que procesa **SIMA Service** para las marcas VW, VW comerciales, AUDI y Skoda, y que abarcan el ciclo de vida del vehículo :  



> **Target de Inspecciones**:   

>> - Primera inspección.  

>> - Siguientes inspecciones.  



> **Target de Otros Servicios**:  

>> - Cambios de correa.  

>> - Cambios de bujías.    

>> - Cambio de líquido de frenos.   

>> - Vencimiento de garantía.  

   

  

 



**¿Qué es una oportunidad?**  



SIMA Service trata como _oportunidad_ la dupla _Vehículo-Cliente_, mostrándola como la ficha de cliente, cuando cumple los siguientes requisitos comunes:  


> - Los clientes relacionados no han manifestado su deseo de no ser contactado.  

>  - Ni el propietario ni el depositario son concesionario o flota.  

> - Los clientes relacionados disponen de teléfono de contacto. 



**SIMA Service** nos muestra las oportunidades según su _fecha estimada de servicio_ de la siguiente manera:    



>**1.** En orden ascendente (de hoy en adelante.  

>**2.** En orden descendente para aquellas ya _vencidas_ como oportunidades.





  

Además también se tiene en cuenta:  

  

 > - El **tiempo medio** de llamada de los clientes tardan para avisar del primer mantenimiento (a los 26000km de media de mercado y no 30000km).  

> - El **kilometraje del último pase** por taller, descartando las tomas hechas durante primer mes tras la entrega.  

> - El **grupo homogéneo** del filtro de aceite, que permite conocer si se ha realizado o no el primer mantenimiento. Si no se hubiera imputado este valor, no se detectaría como primer mantenimiento.      
  

  
## Target de mantenimientos  
  

**Target de mantenimientos** incluye los target de **Primer mantenimiento** y **Siguientes mantenimientos**. Las _oportunidades_ de este target cumplen con los siguientes requisitos específicos: 
 
> - Incluir coches vendidos por el concesionario en los últimos 30 meses.  
> - Kilometraje del vehículo próximo a cumplir 18 meses (o más), o hará 26000 km.  
> - Vehículos que aún no hayan realizado el servicio ni tengan cita para hacerlo.  
    

![Siguiente mantenimiento](images/es-ES_opportunity_nextmaintenances.png)  

    

Para **Siguientes mantenimientos**, se muestran las oportunidades previamente ya contactadas y sobre éstas se recalcula la siguiente información la _Fecha del mantenimiento anterior_ (último mantenimiento) y el _Kilometraje_ (del último registro).       

**SIMA Service** nos facilita actualizar la información de los _Mantenimientos_, según haya sido la respuesta del cliente acerca de un mantenimiento concreto:  

![Mantenimientos](images/es-ES_opportunity_maintenancesbox.png)  


> - Planificado (el cursor sobre el texto mostrará la fecha).  
> - No realizado. 
> - **<span style="color:red; font-family:; font-size:;">Fecha</span>**  pasada para la realización del mantenimiento.
> - **<span style="color:green; font-family:; font-size:;">Fecha</span>** del próximo mantenimiento.  



 


![Recuerde](images/es-ES_remember.png) El plan de mantenimiento para las marcas aquí incluidas es cada 2 años o 30000 kms.    
  
   
 
**TARGET DE OTROS SERVICIOS**  
  
## Cambio de bujías 

Este target afecta únicamente a los _vehículos de gasolina_. Obtiene sus registros de los grupos homogéneos NEZ y NZZ, para visualizar las oportunidades. Las oportunidades en este target:    
  
>   **1.** Cumplen con los requisitos comunes  definidos para los targets.  
> **2.** Incluyen los vehículos cuya _Fecha estimada_ de cambio de correa es dentro de 1 mes.   

La _Fecha estimada_ se calcula en función de uno de los siguientes parámetros:  

> - La fecha de entrega del vehículo  
> - La estimación del kilometraje; por ejemplo, si el vehículo tiene **4 años** o está apunto de llegar a los **60.000kms** según el registro del vehículo.   
> - Las letras de motor.
 
Existe una configuración alternativa de _a los 6 años o 90000kms_ para los motores con letra: aac,aaj.      



## Cambio de correas   

Este target incluye el **Primer cambio de correas** y **Siguientes cambios de correas**. Obtiene sus registros de los grupos homogéneos MFA, MFC y MFS.   

Las oportunidades son mostradas según:  

> - La fecha estimada, calculada en función de la fecha de entrega.  
> - Y el registro de kilometraje, cuando está próximo a los 120.000kms.  
 
   
El **Siguiente cambio de correas** muestra las oportunidades que ya fueron tratadas anteriormente (o con cita) y cuya próxima fecha de cambio es **dentro de 1 mes**. 

![Recuerde](images/es-ES_remember.png) El cambio de correas se debe realizar a los 8 años o 120.000kms.  
   


## Cambio de líquido de frenos    

Este target incluye el **Primer cambio de líquido de frenos** y **Siguientes cambios de líquido de frenos**. Obtiene sus registros del grupo homogéneo CCA.   

Las oportunidades son mostradas según:  

> - La fecha estimada, calculada en función de la fecha de entrega.  
> - El registro de kilometraje, cuando está próximo a los 120.000kms.
> - El primer cambio de líquido de frenos se propone a los 3 años.
 

Además, se propondrá como oportunidad para llamar al cliente a un mes de cumplir el tiempo descrito, mostrándonos la fecha del último cambio de líquido de frenos.



![Recuerde](images/es-ES_remember.png) Los siguientes cambios de líquido se proponen a los 2 años.  

## Vencimiento de garantía   

Este target permite visualizar los clientes cuya garantía (de fabricante o extendida) finalice dentro de 2 meses o menos. Además, se mostrará según los siguientes criterios:  
  
> - Se muestran primero aquellas sin _feedback_ de aceptación.  
> - No son oportunidades aquellos vehículos cuya _fecha de finalización de garantía_ haya pasado.  
> - Se muestran solamente los vehículos vendidos por el propio concesionario.  







