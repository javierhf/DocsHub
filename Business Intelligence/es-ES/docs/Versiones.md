![sima2](images/es-ES_simacanaryversionbn.png)  

Esta página contiene la relación de todas las versiones de la aplicación **BUSINESS INTELLIGENCE** con los cambios, mejoras y correcciones aplicados.   

---      
# Versión 17.RC
  
 - **Se añade el campo** _AppointmentSource_ al _hecho_ _service.FactOrder_.  
 - **Se añade el campo** _Nacionalidad a la _Dimensión_  _common.DimThirdParty_.    
 - **se añade el campo** _Aficiones_ a la dimensión _common.DimThirdPart_.


---      

# Versión 17.07.24  
  
 - **Se añade el campo** _OrderType_ al _hecho_ _parts.FactInvoice_.
 - **Se añaden los campos** _TotalAmount_, _TotalTaxes_, _CurrencyTotalAmount_ y _CurrencyTotalTaxes_ al _hecho_ _sales.FactInvoice_.
 - **Se añade al DataWareHouse una nueva dimensión** _sales.DimContribution_ que contiene información referente al tipo y descripción de las aportaciones y los montantes aferentes.
 - **Se añade al DataWareHouse un nuevo hecho con los datos de aportaciones de concesionarios** registradas para un determinado vehículo, el _hecho_ se denomina _sales.FactDealerContribution_.
 - **Se añade al DataWareHouse un nuevo hecho con los datos de aportaciones reclamadas al importador** por parte de los concesionarios, el _hecho_ se denomina _sales.FactImporterContribution_.

---      
  
# Versión 17.06.15  
  
 - **Se añaden nuevos campos** a la _dimensión DimPart_ y al _hecho PartsFactInvoice_.  
 - **Se añade nuevos campos** a _parts.FactInventory_ en StockPendingDelivery y StockPendingReception.       
 - **Se añade el campo** _Taric_ a la dimensión _DimPart_.
  
---  

  
# Versión 17.06.02  
  
**Se añade una nueva dimensión** al _Hecho de Facturación de Recambios_  para identificar el Asesor comercial de venta de Recambios:    

 > **Tablas de hechos**

 >> parts.FactInvoice  

 > **Tabla de dimensiones**  

 >> parts.DimSalesman (vendedor del Recambio)


**Se añaden nuevos campos** al _Hecho de Proceso de ventas de vehículos nuevos_  para estudiar la detección de necesidades del cliente:  

 > **Tablas de hechos**  
  
 >> sales.FactProcess  
  
 > **Tabla de dimensiones**  
  
 >> - sales.DimSalesman (usuario que toma las necesidades del cliente).   
 
> **Campos**  

>>NeedsDetectionDate
NeedsDetectionLastUpdate
NeedsDetectionCompletionDate
NeedsDetectionCompletionIndicator


**Se añade al DataWarehouse la Detección de Necesidades** en el proceso de ventas de vehículos nuevos, que explotaremos haciendo uso de las siguientes tablas:  
  
> **Tablas de hechos**

>> sales.FactProcessNeedsDetection  
   
> **Tabla de dimensiones**

>> common.DimCompany
common.DimCenter
common.DimThirdParty
common.DimVehicleBrand
common.DimUser
sales.DimProcessContactMotive
sales.DimProcessContactSource
sales.DimProcessDetailedStatus
sales.DimProcessStatus
sales.DimProcessRejectionReason
sales.DimProcessType
sales.DimProcessDigitalPlattform
sales.DimSalesman
 

  
  
--- 
     
  
# Versión 17.04.24    
  
 - **Se añaden los campos** _Grupo_ y _GrupoNombre_ a la Facturación de Recambios, el hecho _parts.FactInvoice_. 
  
 -   **Se añade el campo** _ModelYear_ a la dimensión _DimVehicleProductCatalog_.  
 
 - **Se añade el campo** _parts.FactInvoice_ al nombre del vendedor en _Recambios_.       
 - **Se añade el campo** _IsPPSOPackage_ al hecho de _service.FactJob_ (facturación de taller) y _service.FactInvoice_ (facturación de trabajos) para llevar información sobre PPSO al datawarehouse.   

---  

# Versión 17.03.29     
  
 - **Se ha creado el campo** _PartDescription_ en la dimensión _common.DimPart_ desde la **tabla de origen** _Rec_ReferenciasMaestro_Denominaciones_ y el campo  _Denominacion_.    

--- 

  
# Versión 17.03.22  
  
 - **Se ha creado la dimensión** _common.DimTransactionObject_ a partir de _Gen_Objetos_Transaccion_.         
 - **Se ha añadido el campo** _TransactionObjectKey_ al hecho _service.FactInvoice_ tras unir _TAL_Documentos_SubDetalle.OtranId_ con _Common.DimTransactionObject .OtranId_ y _simaId_.        
 - **Se han añadido los siguientes campos:**  
  
 > - CurrencyUnitPriceTaxExcluded
>> **Equivalente en SIMA:**  _TAL_Documentos_SubDetalle.ImporteBrutoUnitario_Original     
 > - CurrencyTotalPriceTaxExcluded  
>> **Equivalente en SIMA:**  TAL_Documentos_SubDetalle.ImporteBrutoTotal_Origina
 > - CurrencyTotalDiscountTaxExcluded  
>> **Equivalente en SIMA:**  TAL_Documentos_SubDetalle.ImporteDescuentoTotal_Original      
 > - CurrencyTotalAmountTaxExcluded  
>> **Equivalente en SIMA:**  TAL_Documentos_SubDetalle.ImporteNetoTotal_Original   
 > - Currency  
>> **Equivalente en SIMA:** Sio_Documentos_Moneda 
 > -  CurrencyExchangeRate  
>> **Equivalente en SIMA:** Sio_Documentos_History.MonedaCambioservice.FactInvoice            
 > - CurrencyUnitPriceTaxExcluded  
>> **Equivalente en SIMA:**  Rec_Facturas_Clientes_Detalles.DocCurrencyUnitaryGross    
 > - CurrencyTotalPriceTaxExcluded  
>> **Equivalente en SIMA:**  Rec_Facturas_Clientes_Detalles.DocCurrencyGross     
 > - CurrencyTotalAmountTaxExcluded  
>> **Equivalente en SIMA:**  Rec_Facturas_Clientes_Detalles.DocCurrencyNet    
 > - CurrencyTotalDiscountTaxExcluded  
>> **Equivalente en SIMA:**  Rec_Facturas_Clientes_Detalles.DocCurrencyDiscount   
 > - Currency  
>> **Equivalente en SIMA:**  Sio_Documentos_History.Moneda  
 > - CurrencyExchangeRate  
>> **Equivalente en SIMA:**  Sio_Documentos_History.MonedaCambio
  
  
---

# Versión 17.03.15     
  
  
 - **Se ha añadido el campo** _ImporterUsualSupplierName_ e _ImporterUsualSupplierCode_ en la dimensión _DimPart_, para almacenar _nombre/código - id_ del Proveedor habitual para el Importador.    
 - **Se ha creado el campo** _CommonCodeId_ y _CommonCodeDescription_  en la dimensión _DimPart_ (VW).           
 - **Se ha creado el hecho** _service.FactInvoice_ uniendo las tablas _TAL_Citas_History_ con _TAL_Orden_Cabecera_History_ por el campo _CdgCita_.    
 - **Se han añadido los campos** _Tal_Orden_Averias_History.WithMantenainceContract_  en el hecho _service.FactInvoice_.    
 - Se traen las empresas SIMA el histórico _TAL_Citas_.  
 - Se ha unido _Tal_Citas_Hitory.CdgAsesor_ con la dimensión _common.dimUser_ por el campo _UserId_ y _simaId_, 
para almacenar el SKey obtenido en un nuevo campo en _service.FactInvoice_ que se llame _ServiceAdviserSKey_.  
  



---  

  
# Versión 17.02.24  
  
 - Se añade  _ReceptionKilometers_  al hecho _service.FactInvoice_. Este campo corresponde con el kilometraje del vehículo al efectuar la recepción en taller.   
 
 - Se ha cambiado el campo _VehicleAgeAtReceptionen_ a cifra de dos decimales en el hecho _Service.FactInvoice_. Dicho campo corresponde con la antigüedad del coche durante la recepción en el taller.
  
 - Se añaden los siguientes campos a _Opportunity_:  
  
 > - service.FactInvoice con service.DimJobType   
 > - service.FactInvoice con service.DimJobOrigin    

  
 - Se añade un hecho de procesos de ventas de vehículos con su equipamiento, que explotaremos mediante las siguientes tablas:  

 > - Tablas de hechos:  

 >> - sales.FactProcessVehicleEquipment  
  

> - Tabla de dimensiones:  
  
 >> - common.DimCompany   
 >> - common.DimCenter  
 >> - common.DimThirdParty  
 >> - common.DimVehicleBrand  
 >> - common.DimUser  
 >> - sales.DimProcessContactMotive  
 >> - sales.DimProcessContactSource  
 >> - sales.DimProcessDetailedStatus  
 >> - sales.DimProcessStatus  
 >> - sales.DimProcessRejectionReason  
 >> - sales.DimProcessType  
 >> - sales.DimVehicleProductCatalog  
 >> - sales.DimProcessDigitalPlatform  
  


 - Se añaden los siguientes campos  al hecho _sales.FactProcessVehicle_ campos relacionados con el color del vehículo y su interior:  
  
 > - ColorCode  
 > - ColorDescription  
 > - InteriorCode  
 > - InteriorDescription

  
---  
     
    
  
  
# Versión  17.01.26     
  
Se añade el _Inventario de Recambios_  al data warehouse para poder explotarlo con las siguientes tablas:   
  
> - Tablas de hechos:  

>> - parts.FactInventory  
  

> - Tabla de dimensiones:  

>> - common.DimCompany  
>> - common.DimPart  
>> - common.DimthirdParty  
>> - parts.DimWarehouse  
    
Obtener el valor del inventario por marca y almancén, destacando:  
  
 > - Sobrestock (Stock disponible - demanda media mensual * 24 meses.  
 > - Obsoletos.  
 > - Ratio de cobertura (Coste del Inventario / Coste de las ventas) (2.5 meses sería el valor óptimo).  
  
---  

  
# Versión 16.12.12  
  
Se añade un nuevo _hecho_  para poder estudiar a los pedidos de vehículos según su equipamiento:  
  
 > - Tabla de hechos:
>> sales.FactVehicleOrderEquipment  
    

---  

  
# Version 16.11.15  
    
Se añade la _Facturación de Recambios_ al datawarehouse mediante la explitación de las siguientes tablas:    
  
  
>- Tablas de hechos:


>> - parts.FactInvoice
  
> - Tabla de dimensiones:


>> - common.DimCompany
>> - common.DimIssuerCenter
>> - common.DimDocumentType
>> - common.DimthirdParty
>> - common.DimCenter
>> - common.DimDivision
>> - common.DimPart
>> - parts.DimWarehouse
>> - parts.DimChannel
    
  
Se incorporan al  hecho de Pedidos de vehículo los códigos y descripciones de Color e Interior:   
  
 >- Tablas de hechos:

 >> - sales.FactVehicleOrder.ColorCode

 >> - sales.FactVehicleOrder.ColorDescription

 >> - sales.FactVehicleOrder.InteriorCode

 >> - sales.FactVehicleOrder.InteriorDescription
  
---  
  
  
# Version 16.10.24  
  
**NUEVAS FUNCIONALIDADES**    
  
 - Se añaden dos nuevas dimensiones que clasifican los pedidos de vehículos según _Tipo_ (Cliente, Stock) y _Categoría de venta_ (Privado, Demo, Flota, Rent a Car...):  
  
>- Tabla de hechos:    


>>>sales.FactVehicleOrder    


> - Tabla de dimensiones:  


>>>> sales.DimOrderType


>>>>sales.DimOrderCategory  
  
 
---
 


# Versión 16.07.11  

**NUEVAS FUNCIONALIDADES**  
  
 - Mejora la capacidad de planificación mediante el análisis de las ventas en red por periodos de fecha y antigüedad de los vehículos del stock. Se ha añadido:  
 > - Tablas de hechos:  
 >> - sales.FactVehicleOrder  
 >  
 >  - Tabla de dimensiones:  
 >> - common.DimCompany  
 >> - common.DimthirdParty  
 >> - common.DimVehicleBrand  
 >> - sales.DimOrderStatus  
 >> - sales.DimVehicleProdcutCatalogue  
 >> - sales.DimFactory   
   
  
---  

# Versión 16.06.17    

**NUEVAS FUNCIONALIDADES**  

 - Efectividad por marca/modelo/motorización. Se da la posibilidad de explotar la efectividad a nivel de modelo y motorización (familia / modelo del catálogo de producto)    

> - Tablas de hechos:   
>> - sales.FactProcessVehicle
>
> - Tablas de dimensión:
>> - common.DimCompany
>> - common.DimCenter
>> - common.DimThirdParty
>> - common.DimVehicleBrand
>> - common.DimUser
>> - sales.DimProcessContactMotive
>> - sales.DimProcessContactSource
>> - sales.DimProcessDetailedStatus
>> - sales.DimProcessStatus
>> - sales.DimProcessRejectionReason
>> - sales.DimProcessType
>> - sales.DimVehicleProductCatalog

  
---  
  

# Versión 16.05.05


**NUEVAS FUNCIONALIDADES**  

   
 - Se obtiene el número de las acciones planificadas caducadas que están pendientes de cerrar, para poder realizar el seguimiento oportuno. Para ello se miden todas las acciones abiertas con fecha anterior a la fecha actual de explotación del informe. Se han añadido las siguientes tablas y dimensiones:     
   
- Se obtiene la información de clientes potenciales atendiendo a la información suministrada con el alta de clientes, para ser explotada en relación a los hechos de ofertas _sales.FactProcess_.

 
  
---  

# Versión 16.04.20

**NUEVAS FUNCIONALIDADES**  

  - Se incorpora el indicador de prueba dinámica asociado a ofertas para tenerlo en cuenta desde el momento de la planificación de la prueba:  
 >>- Indicador:  _sales.FactProcess.HasTestDrive_    
   

 
 - Análisis de la efectividad de los procesos de venta. Se añaden las siguientes tablas nuevas:    
  
> - Tablas de hechos:  
>> - sales.FactProcess  


> - Tablas de dimensión:  
>> - sales.DimProcessContactMotive  
>> - sales.DimProcessContactSource  
>> - sales.DimProcessDetailedStatus  
>> - sales.DimProcessRejectionReason   
>> - sales.DimProcessStatus  
>> - sales.DimProcessType
  
  
---  

# Versión 16.04.07  

**NUEVAS FUNCIONALIDADES**  
  
 - Se incorpora el análisis de la efectividad de los procesos de venta al DataWarehouse mediante las siguientes nuevas tablas:    
  
>- Tablas de hechos:  
 >>- sales.FactProcess.  
 >  
>  - Tablas de dimensión:  
  >>- sales.DimProcessContactMotive.  
  >>- sales.DimProcessContactSource.  
  >>- sales.DimProcessDetailedStatus.  
  >>- sales.DimProcessRejectionReason.  
  >>- sales.DimProcessStatus.  
  >>- sales.DimProcessType  

---  



# Versión 16.03.23   

**NUEVAS FUNCIONALIDADES**  

 - Segmentación de la facturación de ventas según el domicilio del tercero en España.  
 >>**Nota:** se añaden los campos _Country_, _PostalCode_, _region_, City_ y _Address_.    
  
 - Se añaden los datos de _email_ y _teléfono móvil_ del cliente a los hechos de ventas.   

---  

# Versión 16.03.07    

**NUEVAS FUNCIONALIDADES**

 - Se añaden a la dimensión del vehículo (common.DimVehicle) los atributos:   
 VehicleModel, EngineModelCode yEngineModelDescription.  

>>**Nota:** VehicleModel representa la familia del vehículo. EngineModelCode y EngineModelDescription tendrán los mismos valores que los atributos ya existentes VehicleModelCode y VehicleModelDescription.   
>  
>>Se recomienda modificar los informes actuales que utilicen dichos atributos porque estos últimos atributos serán eliminados en futuras versiones.  

---  

# Versión 16.02.23    

**NUEVAS FUNCIONALIDADES**
  
 - Carga inicial en caliente.  
 - Poder sacar la facturación de un vehículo para calcular el rendimiento según su plan de mantenimiento.
  
---  

# Versión 16.02.11   

**NUEVAS FUNCIONALIDADES** 

 - Incluir número de operaciones y revisar rectificativas.
 - Poder segmentar clientes de ventas en función de datos personales de CRM.  
 
---  



# Versión 16.01.25   

**NUEVAS FUNCIONALIDADES** 

 - Carga de hecho de ventas de vehículos nuevos y usados.  
   
---  
 

# Versiones anteriores   

**NUEVAS FUNCIONALIDADES**
 
  - Carga de hecho de facturación de taller.  
  - Carga de hecho de orden de taller.
  - Carga del hecho de trabajos de taller.  
  - Carga de dimensiones genéricas para los hechos: Terceros, Usuarios, Empresas, entre otras.  
  - Carga de dimensiones de Taller: Talleres, Tipo de servicios, entre otras.   


