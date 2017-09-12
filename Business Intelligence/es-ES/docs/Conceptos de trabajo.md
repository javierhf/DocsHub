![sima2](images/es-ES_simacanaryversionbn.png)   
  ---  
 

## Conceptos  

Para comenzar a **consumir** la información del DataWarehouse es necesario tener en cuenta los siguientes conceptos:  


 - **Tablas de hechos**:  
 >-  Representan los eventos que suceden en un espacio-tiempo concreto y contienen _indicadores/métricas_ que permiten cuantificar y medir los datos cargados como Suma de importes, Nº.de ventas, Top 10 de vendedores, etc. 
 >-  Características: permiten analizar los datos al máximo detalle. 

- **Tablas de dimensiones**:  
>-  Representan la _categoría_ o _clasificación_ sobre los hechos que se quieren medir, es decir, es el prisma mediante el cuál podemos agrupar los datos; por ejemplo, contar el nº. de ventas por año, por país, por cliente, etc.   

El _detalle de las líneas de una tabla de hechos_ es lo que marca su **granuralidad**. Así, observamos que las unidades de medida pueden estar a un nivel de poco detalle (grano grueso) o llegar a un detalle máximo (grano fino).  

A las columnas de la tabla de dimensión se les conoce cómo atributos.
   

## Relaciones entre entidades     

La base de datos del **DataWarehouse** muestra las siguientes relaciones entre entidades:  

   

<table>
<thead>
<tr>
  <th>HECHO</th>
  <th>DIMENSIÓN</th>
</tr>
</thead>
<tbody>
<tr>
  <td>service.FactOrder
</td>
  <td>common.DimCompany <br>common.DimThirdParty</br>
common.DimUser<br>
common.DimVehicle</br>
common.DimVehicleBrand<br>
service.DimOrderStatus</br>
service.DimOrderEconomicStatus<br>
service.DimWorkshop</br>
</td>
</tr>
<tr>
  <td>service.FactJob</td>
  <td>common.DimCompany<br>
common.DimVehicle</br>
common.DimVehicleBrand<br>
common.DimUser</br>
service.DimWorkshop<br>
service.DimJobStatus</br>
service.DimJobEconomicStatus<br>
service.DimJobOrigin</br>
service.DimJobType<br>
service.DimServiceType</br>
</td>
</tr>
<tr>
  <td>service.FactInvoice</td>
  <td>common.DimCompany<br>  
common.DimUser</br>
common.DimVehicle</br>
common.DimVehicleBrand<br>
common.DimDocumentType</br>
common.DimCenter<br>
common.DimDivision</br>
common.DimPart<br>
common.DimThirdParty</br>  
common.DimTransactionObject</br>
service.DimChannel<br>
service.DimServiceType</br>
service.DimWorkshop<br>  
ReceptionKilometers<br>  
service.DimJobType<br> 
service.DimJobOrigin<br>  
</td>
</tr>
<tr>
  <td>sales.FactInvoice</td>
  <td>common.DimCompany<br>
common.DimThirdParty</br>
common.DimCenter<br>
common.DimVehicle</br>
common.DimVehicleBrand</br>
common.DimDocumentType<br>
sales.DimChannel</br>
sales.DimModality
</td>
</tr>
<tr>
  <td>sales.FactProcess</td>
  <td>common.DimCompany<br>
common.DimCenter</br>
common.DimThirdParty<br>
common.DimVehicleBrand</br>
common.DimUser<br>
sales.DimProcessContactMotive</br>
sales.DimProcessContactSource<br>
sales.DimProcessDetailedStatus</br>
sales.DimProcessStatus<br>
sales.DimProcessRejectionReason</br>
sales.DimProcessType</br>  
sales.DimProcessDigitalPlatform</br>    
sales.DimSalesman</br>  
NeedsDetectionDate</br>  
NeedsDetectionLastUpdate</br>  
NeedsDetectionCompletionDate</br>  
NeedsDetectionCompletionIndicato</br>  
NeedsDetectionUserKey</br>  
</td>
</tr>
<tr>
  <td>sales.FactSalesmanAction</td>
  <td>common.DimUser<br>
common.DimCompany</br>
common.DimThirdParty<br>
sales.DimSalesmanActionStatus<br>
sales.DimSalesmanActionResult</br>
sales.DimSalesmanActionSubject<br>
sales.DimSalesmanActionType</br>
</td>
</tr>


<tr>
  <td>sales.FactProcessVehicle</td>
  <td>
common.DimCompany<br>
common.DimCenter<br>
common.DimThirdParty<br>
common.DimVehicleBrand<br>
common.DimUser<br>
sales.DimProcessContactMotive<br>
sales.DimProcessContactSource<br>
sales.DimProcessDetailedStatus<br>
sales.DimProcessStatus<br>
sales.DimProcessRejectionReason<br>
sales.DimProcessType<br>
sales.DimVehicleProductCatalog<br>
</td>
</tr>  

<tr>  
  <td>sales.FactVehicleOrder</td>  
  <td>  
common.DimCompany<br>  
common.DimthirdParty<br>  
common.DimVehicleBrand<br>  
sales.DimOrderStatus<br>  
sales.DimVehicleProdcutCatalogue<br>  
sales.DimFactory<br>   
sales.DimOrderType<br>  
sales.DimOrderCategory<br>  
</td> 
</tr>  
<tr>  
  <td>sales.FactProcessNeedsDetection</td>  
  <td>  
common.DimCompany<br>  
common.DimCenter<br>  
common.DimthirdParty<br>  
common.DimVehicleBrand<br>  
common.DimeUser<br>  
sales.DimProcessContactMotive<br>  
common.DimProcessContactSource<br>  
sales.DimProcessDetailedStatus<br>  
sales.DimProcessStatus<br>  
sales.DimProcessRejectionReason<br>  
sales.DimProcessType<br>  
sales.DimProcessdigitalPlatform<br>  
sales.DimSalesman<br>  
NeedsDetectionDate<br>  
NeedsDetectionLastUpdate<br>  
NeedsDetectionCompletionDate<br>    
 NeedsDetectionCompletionIndicator<br>  
NeedsDetectionUserKey<br>  
Question<br>  
Answer<br>	  
</td> 
</tr>  

<tr>  
  <td>sales.FactVehicleOrderEquipment</td>  
  <td>  
common.DimCompany<br>  
common.DimthirdParty<br>  
common.DimVehicleBrand<br>  
sales.DimOrderStatus<br>  
sales.DimVehicleProductCatalogue<br>  
sales.DimFactory<br>   
sales.DimOrderType<br>  
sales.DimOrderCategory<br>  
</tr> 
</td>  
<tr>  
  <td>parts.FactInvoice</td>  
  <td>  
common.DimCompany<br>  
common.DimIssuer<br>  
common.DimDocumentType<br>  
common.DimthirdParty<br>  
common.DimCenter<br>  
common.DimDivision<br>   
common.DimPart<br>  
parts.DimWarehouse<br>  
parts.DimChannel<br>   
common.DimUser<br>  
common.DimTransactionObject<br>   
parts.DimSalesman<br>
  
  
</tr> 
</td>  
<tr>  
  <td>parts.FactInventory</td>  
  <td>  
common.DimCompany<br>  
common.DimPart<br>  
common.DimthirdParty<br>  
parts.DimWarehouse<br>    
common.DimTransactionObject<br>  

  
  
</tr> 
<tr>  
  <td>sales.FactProcessVehicleEquipment</td>  
  <td>  
common.DimCompany<br>    
common.DimCenter<br>    
common.DimthirdParty<br>     
parts.DimVehicleBrand<br>      
common.DimUser<br>    
sales.DimProcessContactMotive<br>  
sales.DimProcessContactSource<br>  
sales.DimProcessDetailedStatus<br>  
sales.DimProcessStatus<br>  
sales.DimProcessRejectionReason<br>  
sales.DimProcessType<br>  
sales.DimVehicleProductCatalog<br>  
DimProcessDigitalPlatform<br>    


  
  
</tr> 
</td>




</tbody>
</table>  

## Descripción de tablas de dimensiones     
  
 > - **common.DimCompany** -  Maestro que contiene información básica de empresas. No implementa versionado.    
 > - **common.DimThirdParty** - Maestro que contiene información básica de terceros. Implementa versionado.  
 > - **common.DimVehicle** - Maestro que contiene información básica de vehículos. Implementa versionado.  
 > - **common.DimVehicleBrand** - Maestro que contiene información básica de marcas de vehículos. Implementa versionado.  
 > - **common.DimDocumentType** - Maestro que  contiene información acerca de los tipos de documentos de facturación. No implementa versionado.  
 > - **common.DimCenter** - Maestro que  contiene información de los centros de facturación. Implementa versionado.  
 > - **common.DimDivision** - Maestro que  contiene información de las divisiones de facturación. Implementa versionado.  
 > - **common.DimPart** - Maestro que contiene información de las referencias de recambios en facturación. Implementa versionado.     
 > - **common.DimTransactionObject** - Maestro que contiene información de los objetos de transacción en la  facturación de servicios. Implementa versionado.     
 > - **common.DimIssuerCenter** - Maestro que contiene la información básica de los centros emisores.    
 > - **common.DimUser** -  Maestro que contiene información básica de usuarios. Implementa versionado.     
> - **service.DimWorkshop** - Maestro que contiene información básica de taller. Implementa versionado.  
 > - **service.DimJobOrigin** - Maestro que  contiene información acerca del origen de los trabajos. Implementa versionado.  
 > - **service.DimJobType** - Maestro que  contiene información acerca del tipo de los trabajos. Implementa versionado.  
 > - **service.DimJobStatus** - Maestro que  contiene información acerca del estado del trabajo. No implementa versionado.   
> - **service.DimJobEconomicStatus** - Maestro que  contiene información acerca del estado económico del trabajo. No implementa versionado.  
 > - **service.DimOrderStatus** - Maestro que  contiene información acerca del estado de la orden. No implementa versionado.  
 > - **service.DimOrderEconomicStatus** - Maestro que  contiene información acerca del estado de económico de la orden. No implementa versionado.  
 > - **service.DimChannel** - Maestro que  contiene información de canales de pago en facturación de taller. No implementa versionado.  
 > - **service.DimServiceType** - Maestro que  contiene información de los servicios y tipos de servicios de taller en facturación. Implementa versionado.  
 > - **sales.DimChannel** - Maestro que  contiene información de canales de venta en facturación de comercial. No implementa versionado.    
 > - **sales.DimModality** - Maestro que  contiene información del inventario al que pertenece el vehículo. No implementa versionado.      
> - **sales.DimProcessContactMotive** - Maestro que  contiene información del motivo del contacto en el proceso de venta. No implementa versionado.
 > - **sales.DimProcessContactSource** - Maestro que  contiene información del origen del contacto en el proceso de venta. No implementa versionado.     
 > - **sales.DimProcessDetailedStatus** -  Maestro que  contiene información del estado detallado en el proceso de venta. No implementa versionado.   
 > - **sales.DimProcessStatus** -   Maestro que  contiene información del estado en el proceso de venta. No implementa versionado.  
 > - **sales.DimProcessRejectionReason** - Maestro que  contiene información de las razones de rechazo en el proceso de venta. No implementa versionado.    
 > - **sales.DimProcessType** - Maestro que  contiene información de los tipos de proceso de venta. No implementa versionado.    
 > - **sales.DimSalesmanActionStatus**   - Maestro que contiene el estado de la acción del asesor comercial. No implementa versionado.
 > - **sales.DimSalesmanActionResult**   - Maestro que contiene el resultado de la acción del asesor comercial. No implementa versionado.
 > -**sales.DimSalesmanActionSubject**   - Maestro que contiene el asunto de la acción del asesor comercial. No implementa versionado.
 > - **sales.DimSalesmanActionType** - Maestro que contiene el tipo y subtipo de la acción del asesor comercial. Implementa versionado.
 > -**sales.DimVehicleProductCatalog** - Maestro que contiene la información básica de las configuraciones de vehículos respecto del modelo y motorización. Implementa versionado.  
 > - **sales.DimOrderStatus** - Maestro que contiene el estado genérico y el estado detallado del pedido. Implementa versionado.  
 > - **sales.DimFactory** - Maestro que  contiene información de la fábrica dónde se realizan los pedidos de vehículos. No implementa versionado.   
 > - **sales.DimProcessDigitalPlatform** - Maestro que contiene la plataforma digital desde la que se crea la Ofera (Escritorio SIMA/Tablet).     
> - **sales.DimVehicleProductCatalog** - Maestro que contiene la información básica de las configuraciones de vehículos respecto del modelo y motorización. Implementa versionado.  
 > - **sales.DimOrderType** - Maestro que contiene el tipo del pedido (Cliente/Stock). Implementa versionado.    
> - **sales.DimOrderCategory** - Maestro que contiene la categoría del pedido (Privado, Demo, RAC, etc.). Implementa versionado.      
 > - **parts.DimWarehouse** -  Maestro que contiene la información básica de los almacenes de Recambios.  
 > - **parts.DimChannel** - Maestro que contiene la información básica de los canales de venta de Recambios.    
 > - **parts.DimSalesman** - Maestro que contiene información básica de asesores comerciales de venta de Recambios. Implementa versionado.  
 > - **sales.DimSalesman** - Maestro que contiene información básica de asesores comerciales de Ventas de vehículos. Implementa versionado.     


## Tablas de hechos    

  
 > - **service.FactOrder** - Tabla de hechos con los datos de cabecera de la orden. No implementa versionado.  
 > - **service.FactJob** - Tabla de hechos con los datos de los trabajos/averías de la orden. No implementa versionado.  
 > - **service.FactInvoice** - Tabla de hechos con los datos de facturación a nivel de avería e imputaciones de taller. No implementa versionado.  
 > - **sales.FactInvoice** - Tabla de hechos con los datos de facturación a nivel de venta de vehículo. No implementa versionado.  
 > - **sales.FactProcess** - Tabla de hechos con los datos del proceso de venta a nivel de cabecera de la oferta.
 > - **sales.FactSalesmanAction** -  Tabla que contiene los datos de la acciones del asesor comercial. Implementa versionado.
 > - **sales.FactSaleProcessVehicle** - Tabla de hechos con los datos del proceso de venta a nivel de modelo y motorización (familia y modelo) de la oferta.  
 > - **sales.FactVehicleOrder** - Tabla de hechos con los datos de los pedidos de vehículos.  
 > - **sales.FactVehicleOrderEquipment** - Tabla de hechos con los datos de los pedidos de vehículos y su equipamiento.      
 > - **parts.FactInventory** - Tabla de hechos que contiene los datos del Inventario de Recambios.  
 > - **parts.FactInvoice** - Tabla de hechos que contiene los datos de la Facturación de Recambios.
 > - **sales.FactProcessVehicleEquipment** - Tabla de hechos con los datos de procesos de venta de vehículos con su equipamiento.    
 - **sales.FactProcessNeedsDetection** - Tabla de hechos con los datos de detección de necesidades del cliente  (preguntas y respuestas) tomados en el proceso de venta.








 

 
