![sima2](images/en-EN_simacanaryversionbn.png)  

## Concepts  

Before estart **consuming** the information provided by the data warehouse it is necessarylearn the following concepts:


 - **Tables of facts**:   
 >- Tables representing events that took place in a certain space-time and that contains _indicators/metrics_ to quantify and mesure the loaded data (for example, Total of sales, Number of sales, Salesman top 10, etc).
 >-  Characteristics: those tables enables an in-deep analyse.    
 >- The details of the rows in a _table of facts_ set its **granularity**. **BI** measures it for units having a low level of detail (big grain) or a maximum level of detail (small grain). 
>-  Tables representing the _category/ranking_ about measurable facts, in other words, offer us a perspective for data grouping (Sales/Year, Sales/Country, Sales/Customer, etc)
 >- Tables representing events that took place in a certain space-time and that contains _indicators/metrics_ to quantify and mesure the loaded data as, for example, Total of sales, Number of sales, Salesman top 10 etc.
 >-  Characteristics: those tables enables an in-deep analyse.

- **Tables of dimensions**:  


The details of the rows in a _table of facts_ sets its **granularity**. **BI** measures it for units haveing a low level of detail (big grain) or a maximum level of detail (small grain).  

Tha columns in a dimension table are known as attributes.
   

## Relations between entities     

The database of the **DataWarehouse** has the following relations between entities:  

   
<table>
<thead>
<tr>
  <th>HECHO</th>
  <th>DIMENSION</th>
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
sales.DimProcessType<br>  
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
</tr> 
</td>   
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




</tbody></table>   

  
## Description of table of dimensions  
 
  - **common.DimCompany** -  Master containing basic information about enterprises. Does not implement versioning.     
  - **common.DimThirdParty** - Master containing basic information of Third parties. Implements versioning.  
  - **common.DimVehicle** - Master containing basic information of vehicles. Implements versioning.    
  - **common.DimVehicleBrand** - Master containing basic information of brands of vehicles. Implements versioning.  
  - **common.DimDocumentType** - Master containing basic information about the type of invoicing documents. Does not implements versioning.  
  - **common.DimCenter** - Master containing information of the invoicing centers. Implements versioning.  
  - **common.DimDivision** - Master containing information of invoicing divisions. Implements versioning.  
  - **common.DimPart** - Master containing information of references of parts in invoicing. Implements versioning.     
  - **common.DimTransactionObject** - Master containing information of trasaction objects in the invoicing of services. Implements versioning.     
  - **common.DimIssuerCenter** - Master containing basic information of the issuer centers.    
  - **common.DimUser** -  Master containing basic information of users. Implements versioning.     
  - **service.DimWorkshop** - Master containing basic information of workshop. Implements versioning.  
  - **service.DimJobOrigin** - Master containing information about the source of jobs. Implements versioning.  
  - **service.DimJobType** - Master containing information about the type of jobs. Implements versioning.  
  - **service.DimJobStatus** - Master containing information about  the state of the job. Does not implement versioning.   
  - **service.DimJobEconomicStatus** - Master containing information about  the financial state of the job. Does not implement versioning.  
  - **service.DimOrderStatus** - Master containing information about  the state of the order. Does not implement versioning.  
  - **service.DimOrderEconomicStatus** - Master containing information about  the financial state of the order. Does not implement versioning.  
  - **service.DimChannel** - Master containing information about  the payment channels in workshop invoicing. Does not implement versioning.  
  - **service.DimServiceType** - Master containing information about the types of workshop services in invoicing. Implements versioning.  
  - **sales.DimChannel** - Master containing information of the invoicing channels os sales. Does not implement versioning.    
  - **sales.DimModality** - Master containing information of the inventory where the vehicles belongs. Does not implement versioning.      
  - **sales.DimProcessContactMotive** - Master containing information of the motive of contact in the sales process. Does not implement versioning.
  - **sales.DimProcessContactSource** - Master containing information of the origin of contact in the sales process. Does not implement versioning.     
  - **sales.DimProcessDetailedStatus** -  Master containing information of the in-detail state in the sales process. Does not implement versioning.   
  - **sales.DimProcessStatus** -   Master containing information of the state in the sales process. Does not implement versioning.  
  - **sales.DimProcessRejectionReason** - Master containing information of the rejection reasons in the sales process. Does not implement versioning.    
  - **sales.DimProcessType** - Master containing information of the types of sales process. Does not implement versioning.    
  - **sales.DimSalesmanActionStatus**   - Master containing the state of the action of the sales adviser. Does not implement versioning.
  - **sales.DimSalesmanActionResult**   - Master containing the result of the action of the sales adviser. Does not implement versioning.
  -**sales.DimSalesmanActionSubject**   - Master containing the subject of the action of the sales advisor. Does not implement versioning.
  - **sales.DimSalesmanActionType** - Master containing the type and subtype of the action of the slaes advisor. Implements versioning.
  -**sales.DimVehicleProductCatalog** - Master containing the basic information of the configuration of the vehicles related to model and engine. Implements versioning.  
  - **sales.DimOrderStatus** - Master containing the generic state in-detail. Implements versioning.  
  - **sales.DimFactory** - Master containing information of the factory where the orders are made. Does not implement versioning.   
  - **sales.DimProcessDigitalPlatform** - Master containing the digital platform that has creates the offer (SIMA desktop/Tablet).     
  - **sales.DimVehicleProductCatalog** - Master containing the basic information of the vehicles configurations related to model and engine. Implements versioning.  
  - **sales.DimOrderType** - Master containing the type of order (Customer/Stock). Implements versioning.    
  - **sales.DimOrderCategory** - Master containing the order category (Private, Demo, RAC, etc.). Implements versioning.      
  - **parts.DimWarehouse** -  Master containing the basic information of the parts warehouses.  
  - **parts.DimChannel** - Master containing the basic information of the sales channels of parts.   
 - **parts.DimSalesman** - Master containing basic information about the sales advisers of Parts sales. Implements versioning.   
 - **sales.DimSalesman** - Master contaning basic information about the sales advisers of vehicles sales. Implements versioning.      
  

## Tables of fact    

  
- **service.FactOrder** - Table containing data of the header of the order. Does not implement versioning.  
- **service.FactJob** - Table containing data of the jobs/damages of the order. Does not implement versioning.  
- **service.FactInvoice** - Table containing invoicing data at a damage/imputation of workshop level. Does not implements versioning.
- **sales.FactInvoice** - Table containing invoicing data at a vehicle sales level. Does not implement versioning.  
- **sales.FactProcess** - TAble containing data of the sales process at a offer header level.
- **sales.FactSalesmanAction** -  Table containing data of the salesman actions. Implements versioning.
- **sales.FactSaleProcessVehicle** - Table containing data of the sales porcess at a model and engine (family and model of the order) level.
- **sales.FactVehicleOrder** - Table containing data of the vehicle orders.  
 - **sales.FactVehicleOrderEquipment** - Table of facts containing orders data accordgin to their equipment.  
- **parts.FactInventory** - Table of facts containing data from the Parts Inventory.  
- **parts.FactInvoice** - Table of facts containing data from the Parts Invoicing.    
 - **sales.FactProcessVehicleEquipment** - Table of facts containing the data of the sales process of the vehicles including their equipment.    
- **sales.FactProcessNeedsDetection** - Tablae of facts containing data from theneeds detetion of the customer (questions and answers) extracted from the sales process.      

