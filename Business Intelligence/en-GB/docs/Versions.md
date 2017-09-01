![sima2](images/en-EN_simacanaryversionbn.png)  

This page details the major additions and changes in each feature released of **BUSINESS INTELLIGENCE**.   

---      
# Versión 17.RC
  
 - **New field** _AppointmentSource_ has been added to _fact_ _service.FactOrder_.   
 - **New field** _Nationality_ has been added to _Dimension_   _common.DimThirdParty_.      
 - **New field** _Hobbies_  has been added to _Dimension_common.DimThirdPart_.  

---        

# Version 17.07.24  
  
 - **New field** _OrderType_ has been added to _fact_ _parts.FactInvoice_.  
 - **New fields** _TotalAmount_, _TotalTaxes_, _CurrencyTotalAmount_ and _CurrencyTotalTaxes_ have been added to _fact_ _sales.FactInvoice_.
 - **A new dimension has been added to DataWareHouse** _sales.DimContribution_ which contains information regarding the type and description of the contributions and the amounts.
 - **A new fact has been added to DataWareHouse with the data of dealer's contributions** for a vehicle, the _fact_ is _sales.FactDealerContribution_.
 - **A new fact has been added to DataWareHouse with the data of contributions claimed to the importer** from the dealers, the _fact_ is _sales.FactImporterContribution_.

---        
  
# Version 17.15.06  
  
 - **New fields have been added** to _dimension DimPart_ and to the _fact PartsFactInvoice_.  
 - **New fields have been added** to _parts.FactInventory_ in StockPendingDelivery and StockPendingReception.     
 - **New field** _Taric_ has been added to dimension _DimPart_.  
  
---    
  
# Version 17.06.02  
  
**A new dimension has been added** to the _Fact of Parts Invoicing_ to identify the salesman of parts sales:

 > **Table of facts**

 >> parts.FactInvoice  

 > **Table of dimensions**  

 >> parts.DimSalesman (parts salesman)


**New fields have been added** to teh _Fact of Sales Process for new vehicles_  to study needs detection of the customer:

 > **Table of facts**  
  
 >> sales.FactProcess  
  
 > **Table of dimensions**  
  
 >> - sales.DimSalesman (user gather customer needs detection).   
 
> **Fields**  

>>NeedsDetectionDate
NeedsDetectionLastUpdate
NeedsDetectionCompletionDate
NeedsDetectionCompletionIndicator


**Needs Detection has been added to the DataWarehouse** to the sales process of new vehicles. To exploit it we will be using these tables:  
  
> **Table of facts**

>> sales.FactProcessNeedsDetection  
   
> **Table of dimensions**

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
  

 - **It has been added the fields** _Grupo_ and _GrupoNombre_  to the invoicing of Parts, the  fact _parts.FactInvoice_.   
  
 -   **It has been added the field**  _ModelYear_ to dimension _DimVehicleProductCatalog_.  
 
 - **It has been added the field** _parts.FactInvoice_ to the name of the salesman in _Parts_.         
 - **It has been added the field** _IsPPSOPackage_  to the fact _service.FactJob_ (workshop invoicing) and _service.FactInvoice_ (jobs invoicing) so that it is possible to check PPSO information in the data warehouse.  
  
---  
  
  
# Version 17.03.29    
  
 - **It has been added the field** _PartDescription_ in dimension _common.DimPart_ from the **source table** _Rec_ReferenciasMaestro_Denominaciones_ and the field  _Denominacion_.    

---  

  
# Version 17.03.22  
  
 - **It has been added the dimension** _common.DimTransactionObject_ from _Gen_Objetos_Transaccion_.         
 - **It has been added the field** _TransactionObjectKey_ to the fact _service.FactInvoice_ from the union of  _TAL_Documentos_SubDetalle.OtranId_ with _Common.DimTransactionObject .OtranId_ and _simaId_.        
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

# Version 17.03.15     
  
  
 - **It has been added the filed** _ImporterUsualSupplierName_ and _ImporterUsualSupplierCode_ in dimension _DimPart_ to save _nombre/código - id_ of the regular provider of the Importer.    
  
 - **It has been added the filed** _CommonCodeId_ and _CommonCodeDescription_  in dimensions _DimPart_ (VW).           
 - **It has been added the fact** _service.FactInvoice_ from the union of tables _TAL_Citas_History_ with _TAL_Orden_Cabecera_History_ by the field _CdgCita_.    
 - **It has been added the filed** _Tal_Orden_Averias_History.WithMantenainceContract_  in the fact _service.FactInvoice_.    
 - SIMA enterprises are retrieve from the history _TAL_Citas_.  
 - **It have been united** _Tal_Citas_Hitory.CdgAsesor_ with dimension _common.dimUser_ y the field _UserId_ and _simaId_, to save the SKey obtained en a new field in _service.FactInvoice_  named as _ServiceAdviserSKey_.  
  



  
  
---      
  
# Version 17.02.24 
  
 - The fact  _service.FactInvoice_  is added the field _ReceptionKilometers_ containing the kilometers of the vehicle at the moment of receptioning in the workshop.  
 
 - The field _VehicleAgeAtReceptionen_ has ben modified in the fact _Service.FactInvoice_, containing the age of the vehicle during the receptioning of the workshop. 
  
 - The following fields have been added to _Opportunity_:  
  
 > - service.FactInvoice con service.DimJobType   
 > - service.FactInvoice con service.DimJobOrigin    
  
 - The fact _sales.FactProcessVehicleEquipment_  is added to be exploited from these tables:  

 > - Tables of facts:  

 >> - sales.FactProcessVehicleEquipment  
  

> - Table of dimensions:  
  
 >> - common.DimCompany   
 >> - common.DimCenter  
 >> - common.DimThirdParty  
 >> - common.DimVehicleBrand  
 >> - ommon.DimUser  
 >> - sales.DimProcessContactMotive  
 >> - sales.DimProcessContactSource  
 >> - sales.DimProcessDetailedStatus  
 >> - sales.DimProcessStatus  
 >> - sales.DimProcessRejectionReason  
 >> - sales.DimProcessType  
 >> - sales.DimVehicleProductCatalog  
 >> - sales.DimProcessDigitalPlatform  
  


The fact _sales.FactProcessVehicle_ includes now the followgin new fileds for color and interior:  
  
 - ColorCode  
 - ColorDescription  
 - InteriorCode  
 - InteriorDescription   
  
---  

  

# Version  17.01.26     
  
The fact _Parts inventory_ is added  to the data warehouse in order to exploit the following tables:
  
> - Table of fact:  

>> - parts.FactInventory  
  

> - Table of dimensions:  

>> - common.DimCompany  
>> - common.DimPart  
>> - common.DimthirdParty  
>> - parts.DimWarehouse  
  
Now it's possible to calculate the value of the inventory by brand and warehouse, underlining:  
  
 > - Overstockage (available stock - monthly average demand * 24 months).  
 > - Obsoletes.  
 > - Coverage ratio (Inventory costs/ Sales costs) (2.5 months as optimus value).    
  
---  
  
  
  
  
# Version 16.12.12  
  
A new _fact_ is added ni order to study orders according to their equipment:  
  
> - Table of facts:
sales.FactVehicleOrderEquipment      
  
---
  
  
# Version 16.11.15  
    
_Parts invoicing_ has been added to the datawarehouse to be exploited within the following tables:  
  
>- Tables of facts:


>> - parts.FactInvoice
  
> - Table of dimensions:


>> - common.DimCompany
>> - common.DimIssuerCenter
>> - common.DimDocumentType
>> - common.DimthirdParty
>> - common.DimCenter
>> - common.DimDivision
>> - common.DimPart
>> - parts.DimWarehouse
>> - parts.DimChannel    
  
Codes and descriptions of Color and Interior have been added to the table of Orders of vehicles:   
  
 >- Table of facts:

 >> - sales.FactVehicleOrder.ColorCode

 >> - sales.FactVehicleOrder.ColorDescription

 >> - sales.FactVehicleOrder.InteriorCode

 >> - sales.FactVehicleOrder.InteriorDescription

  ---  

# Version 16.10.24  
  
**NEW FEATURES**    
  
 - Two new dimensions have been added to classify the orders of vehicles according to _Type_ (Customer, Stock and _Category of sales_ (Private, Demo, Fleet, Rent a Car...):  
  
>- Table of facts:    


>>>sales.FactVehicleOrder    


> - Table of dimensions:  


>>>> sales.DimOrderType


>>>>sales.DimOrderCategory  

  
---  
  


# Version 16.07.11  

**NEW FEATURES**  
  
 - Planning capacity improves due to the analysis of network sales for date ranges and time in stock.  
  
 > - Tables of facts:  
 >> - sales.FactVehicleOrder  
 >  
 >  - Table of dimensions:  
 >> - common.DimCompany  
 >> - common.DimthirdParty  
 >> - common.DimVehicleBrand  
 >> - sales.DimOrderStatus  
 >> - sales.DimVehicleProdcutCatalogue  
 >> - sales.DimFactory   
   
  
---    

   

# Version 16.06.17    

**NEW FEATURES**  

 - Offers effectiveness is now measured by brand, model and engine (family / model of the product catalogue).    

> - Tables of fact:   
>> - sales.FactProcessVehicle
>
> - Tables of dimension:
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
     

   

# Version 16.05.05  

**NEW FEATURES**  

   
    
 - The number of scheduled and expired close-pending actions is calculated to allow the related follow-up process. To do so, open actions dated before the current date of report's exploitation are measured. The following tables and dimensions have been added:  
   
 >> - Table of facts:  
 >>> - sales.FactSalesmanAction  
 >      
 >> - Tables of dimensions:  
 >>> - sales.DimSalesmanActionStatus  
 >>> - sales.DimSalesmanActionResult  
 >>> - sales.DimSalesmanActionSubject  
 >>> - sales.DimSalesmanActionType   
   
- Information about potential customers is obtained from the information of the customer's registration to be exploited in the facts of offers _sales.FactProcess_.
 
 --- 

# Version 16.04.20

**NEW FEATURES**  

 - Test drive indicator is added and associated to offers to be taken into account at the moment of scheduled a test drive:  
 >>- Indicator:  _sales.FactProcess.HasTestDrive_.  
   
- Efficiency analysis for the sales process. The following tables have been added:  
    
 
> - Table of facts:  
>> - sales.FactProcess  



> - Table of dimension:  
>>- sales.DimProcessContactMotive  
>>- sales.DimProcessContactSource  
>>- sales.DimProcessDetailedStatus  
>>- sales.DimProcessRejectionReason   
>>- sales.DimProcessStatus  
>>- sales.DimProcessType    

  
  

---   

# Version 16.04.07  

**NEW FEATURES**  
  
 - Efectiveness analysis of sales process in the data warehouse with the addiotion of the following tables:
 >- Table of facts:  
 >>- sales.FactProcess.  
 >  
  - Table of dimensions:  
  >>- sales.DimProcessContactMotive.  
  >- sales.DimProcessContactSource.  
  >- sales.DimProcessDetailedStatus.  
  >- sales.DimProcessRejectionReason.  
  >- sales.DimProcessStatus.  
  >- sales.DimProcessType  
   
 
---  
  
# Version 16.03.23   

**NEW FEATURES**  

 - Sales invoice is segmentated according to the address of the third party in Spain.  
 >>**Note:** Fields of _Country_, _PostaCode_, _region_, City_ and _Address_ has been added.    
 
 - _Email_ and _cell phone number_ have been added to sales fact.  


---  
 

# Version 16.03.07 
  
**NEW FEATURES**  

 - New attibutes added to **common.DimVehicle** (common.DimVehicle):  _VehicleModel_, _EngineModelCode_ y _EngineModelDescription_.   
 >>-  **Note**:  _VehicleModel_ represents the famiy of vehicle. _EngineModelCode_ y _EngineModelDescription_ have the same values than the current attibutes _VehicleModelCode_ y _VehicleModelDescription_.   
>  
>>It 's higly recommended to modify those reports currently using the previous attributes because this attributes will be removed in coming versions.




---  

# Version 16.02.23  
  
 - Initial data load of the data warehouse in Real-Time.  
 - Workshop invoicing to calculate the performance of vehicle maintenance plans.

---  

# Version 16.02.11  

 - Number of operations and adjusting operations are now included.
 - Segmentation for sales customer according to CRM personal data.
 
---  



# Version 16.01.25  

 - Load of New and Used vehicles facts.
   
---  
 

# Previous versions  


 
  - Load of Workshop invoicing fact.  
  - Load of Workshop order fact.
  - Load of Works of Workshop fact.  
  - Load of Generic dimensions for facts: Third parties, Users and Enterprises among others.  
  - Load of Workshop dimensions: Workshops, Type of services, etc.   


