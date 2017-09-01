![Sima2 Canary version](Images/en-EN_simacanaryversionbn.png)  
 

This page shows all the versions published of **Ordering**.  
  
Subscribe this **changelog page**, to receive _what's new_: Click [Subscribe](http://eepurl.com/cZkO45) 

---      
  
# Version 17.08.28    
  
**GENERAL FEATURES**  
  
 - Management of the different _Sources_ sent by Nadin.  
 - Processing of WE for _weights_ and _emissions_.  
  
**ORDER DETAILS**  
  
 > **WLTP Notifications**  
 >> - WLTP data is coloured in red when modified in the last 7 days.    

  
**IMPROVEMENTS**  
  
 - **Ordering** shows a message notifying the user that the product catalogue is not in the user's language.
  
---  


# Version 17.08.14  
  
**GENERAL FEATURES**  
  
 - New page of **Subscribe me** in the user documentation to subscribe and unsubscribe from the list of the new version email. Subcribe option is also available from the **Versions** page.  

**ORDER DETAILS**   

 - Get and visualize WLTP data coming from Nadin after a check against Manufacturer.
 - Save WLTP data that were obtained from a check against Manufacturer and  saving them in the order.
 - Update WLTP data that were send by the Importer's tools and associat them with the order.    
  
**TRANSFERS**  

 - Request confirmation when Accepting or Rejecting a transfer request.  
 - Accept transfers requests of orders and move the order to the new dealer.  
 - Make the transfer of the order when accepting the transfer request.    
 - Accept/Reject options on order requests are blocked of order state "Not found".    
  
---    

# Version 17.07.28
  
 - Communication management to Nadin improved when other sinchronization processes have not been finished.
 - Sending Delivery to customer data to Nadin when complete process is finished.
 - Users with specific rights can recover a vehicle from Archive (also in Nadin) to active vehicles.
 - Check the configuration before saving a new order when orders are created consecutively.
 - Communication management to Nadin improved when customer is not saved previously in Nadin.
 - Processing information of WLTP data which could be received from Nadin when a FAVAS CHECK is executed.
 - Improvement of sell date and arrival to dealer date so sell date cannot be lower than arrival dealer date.
 - Availability to define that delivery date must be the current date and no other previous dates.

***    
  
# Versión 17.06.21    
  
 - Control processes of information synchronization with the importer, avoiding losing information not previously sent to the importer's application.  
 - Send a change of visibility.   
 - Manage permissions to recover orders of the history.    
  
---
  
# Version 17.06.20   
  
**GENERAL FEATURES**    

 - Remove an order, communicating with Nadin, and noting the errors while removing according to the Importer response (Nadin).    
 - Send plate data when saving  the information of the delivery.  
  
**ORDER DETAILS**    
  
 -  Send remove request to Nadin for orders in this status:  _NewPending_ (0080), _Stored_ (0090), _ImpSec_ (0100), _Ordered_ (0200), _Order Cancelled_ (0275), _Frozen_ (0280) and _Scrapped_ (2700).    
 - Send Nadin the customer assignation of customer, salesman, agent and type of sale.       
 - Modify an order without description.  
 - Show equipment in the order details.  
 - Send plate information when saving delivery information.  
  
**CANCELLATIONS**  
  
 - Check cancellation notifications for my orders.    
  
**ORDERS ARRIVAL**  
  
 - Visualize salesman and customer in the lists.    
  
**MANAGEMENT OF PERMISSIONS**  
  
 - Cancellation permissions management.     
  
**FIXES**  
  
**General fix**  
  
 - Error was shown when loading the page and web navigation changed from https to http.  
  
**Order details**  
  
 - Equipment were not being shown in the order details.
  
---  

# Version 17.05.24

**NEW FEATURES**

**DASHBOARD**

* Send orders to Nadin from the menu option and Notifications panel _Orders pending to deliver_.

**DELIVERIES**

* Send an order to Nadin.
* An order is not send directly to factory if there is a manufacturer error.
* Send modification to Importer
* Modify an order already sent.
* Test sending Order request just with the order number.
* Send a _NO_ and process the answer.
* Update the order with the next order number available, if an error 18 appears when sending a _OE(N)_.
* Obtain the next order number available in Nadin.

**SETTINGS: USERS MANAGEMENT**

> **Permissions management**

>>

* Manage the send orders permission when editing users.

**FIX**

  - Model base configuration is available if there are not available versions.          
  - Track all compulsories range considering all possible combinations.  
  - Inform the user when a selected vehicle does not have History.
***

# Version 17.04.11

**NEW FEATURES**

> **Configurator**

* _Vehicles search_ box searches by equipment code in the list of orders.
* Existing equipment is taken to the new version even if it is unavailable, in the following cases:
 
>> - Family description out of valid date.
>> - Equipment description out of valid date.
>> - Relationship with model out of valid date.
>> - There is no relationship or no definition for that model.

**New order**

* SNR equipment family multiple choice is available.
* Equipment is added to the version even if they do not show any family information.

**Orders delivery pending**

* Send arrival confirmation to Importer.

**IMPROVEMENTS**

* Legibility in error information display.

**FIXES**

> **Edit order**

>>

* Model is retrieved when editing an order.

**New order**

>>

* Version deleteable equipment is controlled when making an order.

***

# Version 17.03.17

**NEW FEATURES**

> **Details of vehicle**

>> **Remarks**

* Remarks are editable, both internal and external.

**IMPROVEMENTS**

* Validation summary text of an order is more legible and clarifies the useful information for the user.

***

# Version 17.03.09

**NEW FEATURES**

* Check information in the Importer about a vehicle in our dealer.
* Errors of an order send from the Importer are now processed.

> **Details of vehicle**

>> **Transport information**

* Transport information is now shown in the details of the vehicle and associated to that vehicle.

**Remarks**

* Internal and shared-with the Importer remarks are shown in the details of a vehicle.

**IMPROVEMENTS**

* Communication process with the Importer.

**FIXES**

* Registration date were shown disabled.
* Importer system is now checkable, only for my active vehicles and not-delivered-to-customer vehicles.

***

# Version 17.02.14

**NEW FEATURES**

> **Create order**

>>

* Check order against factory before saving it. This option is only valid for users with access permissions to factory.

**Order details**

>>

* Visualize sold vehicles as demo vehicles associated with the customer.
* Check the current state of an order by communicating with Nadin (manufacturer) the last changes of the order.
* Receive and process the OT received of Nadin.
* Process the OT of Nadin.

**Lists of orders.**

>>

* Order state can be checked against my dealer, even if the state is different of Deleted or _Modification pending_.
* Compulsories defined in different registers are now considered in those cases with more than 1 compulsory register.

**IMPROVEMENTS**

* Dashboard interface and menu buttons.
* Registration request in Portugal.
* Permissions translation.

***

# Version 16.12.23

**NEW FEATURES**

> **Settings: user management**

>>

* Permissions of arrival confirmation are checked for orders to the dealer.
* Assign/Change permissions are available to confirm the arrival of vehicles to the dealer.
* Check permissions to block orders.
* Assign/Change permissions to block orders.

***

# Version 16.12.22

**NEW FEATURES**

> **Permissions management**

* Assign/Change to modify the configuration of an order (edit order).
* Verify user permissions to Accept/Deny a transfer request of an order of a diferent dealer.
* Assign/Change permissions to manage the orders transfer request (create, accept, deny).
* Cannot remove my own user when logged on.

> **Plate management**

* Plate request (Portugal).
* REQ request are not considered when unregistering a vehicle.

> **Orders configuration**

* Model base configuration is available when there are no versions.
* A base model can be retrieved when an order is rebuilt to be modified.

> **Transfer management**

* Visualize a message to cancel the transfer request.

**GENERAL IMPROVEMENT**

>

* Unnecesary translations are removed.

***

# Versión 16.12.13

**GENERAL IMPROVEMENT**

* Accept and Cancel buttons standardized there position in modal windows.

**USED VEHICLES**

* Access the customer details of a vehicle sold as UV (used vehicle).

**PERMISSIONS MANAGEMENT**

* Assign permission to modify only my own orders or any order.
* Check if I have permissions to remove orders.
* Check permissions to send a transfer request against an order of a different dealer.
* Assign permissions to remove only my orders or any orders.

**CUSTOMER PROFILE**

* Show requested fields for create or edit a customer.

**SETTINGS: USER MANAGEMENT**

* Show requested fields in the customer profile.
* Show requested fields when changing my password.

**ORDER DETAILS**

* Block the plate modification and the registration date of a vehicle.

***

# Versión 16.11.25

**SETTINGS: USERS MANAGEMENT**

**New features**

* Verify the permissions of a user for creating orders and blocked orders.
* Assign new default dealer to a user of my dealer.
* Manage orders creation (blocked or not) according to user permissions.
* Inform users when they do not have permissions to create users.
* Edit permissions of orders creation.

**Fixes**

* Model equipment were not loaded after selecting it.

***

# Version 16.11.16

**GENERAL FEATURES**

* Unify the naming of enterprises.
* Publish the images web services.
* Search by vehicle version description in the general searcher.

**SETTINGS: USERS MANAGEMENT**

* Assign user permission management to a user.

**DEMO VEHICLES MANAGEMENT**

* Control and assign a complete unregistration for a demo before delivering the vehicle.

***

# Version 16.11.07

**SETTINGS: USER MANAGEMENT**

* Access control of users.
* Removing permissions for a user when deleting it from a dealer.

**VEHICLE CONFIGURATION**

* Incompatibilities between packages are not considered  (of there is an equipment repeated) when making the order.

***

# Version 16.11.04

**GENERAL FEATURES**

* Register last login access to the dealer of a user.
* Show brand logo if there is no vehicle image in the manufacturer.

**GENERAL IMPROVEMENT**

* Different actions in a form are grouped in a single button.

**DEMO VEHICLES**

**New feature**

* Assign agent to a demo vehicle of my dealer.
* Assign seller to a demo vehicle of my dealer.
* Assign delivery date to a demo vehicle.

**SETTINGS: USERS MANAGEMENT**

**New features**

* Modify user data of my dealer.
* Delete a user from my dealer.
* Mark as _Seller_ a guest user in my dealer.

**LOGIN**

**Fix**

* System control handles the user session vigency so that a system error is not displayed but the notification of session expired.

***

# Version 16.10.11

**GENERAL IMPROVEMENT**

* Format applied to requested fields in forms.

**GENERAL FIX**

* When there is no combination of equipment available appeared an empty message.

**SETTINGS: USERS MANAGEMENT**

> **New features**

* Attach user from a different dealer to my dealer.
* Edit the information of a user of my dealer.

**DEMO VEHICLES**

> **New features**

* Assign sale date.
* Edit a customer assigned to a demo vehicle of my dealer.

***

# Version 16.10.04

**GENERAL IMPROVEMENTS**

* Show brand logo of a vehicle when there is no image available of the vehicle.
* Close session when login in with a different user.

**SETTINGS: USER MANAGEMENT**

> **New features**

* Create new users for my dealer.
* Visualize the users of my dealer.
* Change password.

**ORDER DETAILS**

> **New features**

* Show the TI and the DPW in the order details.
* Assign delivery date to a customer.
* Assign type of sale from the order details.
* Accept a transfer request received.
* Block the modification of vehicle visibility for dealers.
* Show requested fields necessary to complete an order.

**Improvements**

* _Save_ buttons are unified in the sales section.

**CUSTOMER DETAILS**

> **New features**

* Define zip code for the vehicle.

**MODIFY VEHICLE**

> **New features**

* Identify the version equipment unrebuilt.
* Identify version equipment not related with a model.

**DEMO VEHICLE**

> **New features**

* Search my active demo vehicles and sale pending vehicle.
* Assign a new customer to a demo vehicle of my dealer.
* Assign an existing customer to a demo vehicle of my dealer
* Remove customer associated to a demo vehicle of my dealer.

**USED VEHICLE**

> **New features**

* Search my inactive demo vehicle sale pending.

***

# Version 16.08.29

**NEW FEATURES**

* Received multiple requests of transfer on a single order.

**Customer management**

>

* Menu for customer management of my dealer.
* Search customers of my dealer.
* Visualize orders associated to a customer.
* Show vehicles of the customers of my dealer (active associated orders and in the History).

**Order details**

>

* Mark customers as _disabled_ to prevent associate them to an order.
* Assign salesman.
* Visualize manufacturer errors with its code and description in the order details.
* Visualize equipment and their description grouped by type of equipment (version, optionals, serie).
* Access Orders details from the details page _for models not availables_.
* Access Order details from Sent transfer requests.
* Show equipment grouped and their description from _See more_ button.
* Assign salesman from the Order details page of my orders.

**Order history*

>

* Visualize the history of changes of an order.

**Modify orders*

>

* Catalogue rules are applied on orders in the state of _Saved Desy_ when modifying orders, except for those modifications of _version equipment unrelated to the model_ and _out of date version equipment of the associated model_. Next deployments.

**Configure an order*

>

* Visualize the previous vehicle configuration of a vehicle on the modification page.

**IMPROVEMENTS**

* Dealers selector shows dealers in chronological order.
* Visualize the dealers code and their additional description (tooltip) on the net orders list.
* Show received requests on a Pending state.
* Checking the modification and removing of dates.

***

# Version 16.07.08

**NEW FEATURES**

* Remove orders, Remove orders (individually or masivelly) in state of _Not found_, _Deleted_ y _Order cancelled_.
* Show my transfer requests sent.
* Request a transfer of a visible order of a different dealer.
* Show requests for a vehicle in the vehicle details page.<br>
Reject a request from another dealer again my orders.
* Cancel a request of a net order.
* Cancelled transfer requests and Accepted transfer requests are not considered when requesting a transfer again.
* Filter by state the sent requests.
* Show rejected requests.
* Edit a customer from the order details.
* Net order in state of In error or In Warning are not shown, if my user is a dealer.
* Create new customer is blocked for stock orders.

***

# Version 16.06.17

**NEW FEATURES**

* Check plates mask: system will check the mask of active plates. Plates have to be written in capitals as defined in the plate's mask.
* Edit the customer associated to an order from the details of the order. Including modification and queueing for communication in the importer system (Nadin  for VW Group).

**IMPROVEMENTS**

* Block New Customer button while creating an order when selecting the order as stock.
* Deployment process of the application so integrated authentication changes are applied with the domain.
* Block design style is apply to the page of Order Details.
* Apply different colors for each type of notifications on the Dashboard.

***

# Version 16.06.09

**NEW FEATURES**

* A report about the stock orders is displayed on the dashboard, grouped by model. Mark and unmark model groups is available.
* Block changes for a vehicle with a state preventing changes.
* Change plate and registration plate date of a vehicle.
* Set date of sales for a vehicle.
* Search in the History of orders.
* Access details page of an order in the History page.
* If vehicle is not found, it is possible to search it in the History page and viceversa.

**IMPROVEMENTS**

* Verify that users cannot configure base models if they do not have permissions.
* Adjust the details of an order to improve layout homogeneity.

***

# Version 16.05.17

**NEW FEATURES**

* Base models cannot be used for a configuration in dealers.
* Select the type of sales of the order.
* Type of error is shown on the page of **Orders in error**.
* Timing-indicator (week of production) code is included in the **Configurator**.
* Modelgroup and model codes are included in the **Configurator**.
* NADIN errors are shown in the page of **Orders in error** in the language selected of the user.

**IMPROVEMENTS**

* Notifications are sorted by its importance and notification on 0 are hidden.

***

# Version 16.05.05

**NEW FEATURES**

* Access the Details of an order. Type of order is identified (net customer and my customers) and its visibility.
* Create a new customer and associate it to an order. Check for customer duplicity.
* Simplifing the changing process of the customer assigned to an order. Visibility is not affected.
* Keep the original date of contract.
* Remove a customer assignated to an order.
* Change visibility of an order.
* Assign visibility to an order after removing the customer.
* Adjust date format according to the settings of the customer.
* Checking customer potentially duplicated. Customer information is included to avoid duplication, so that we can identify the right customer.

**IMPROVEMENTS**

* Vehicle image is displayed on the page of **New order**.




