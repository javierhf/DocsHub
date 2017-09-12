![sima2](images/en-EN_simacanaryversionbn.png)  

   
This page details the major additions and changes in each feature released of **SIMA Service**.      
  
---    

# Version 17.08.29  
  
**CROSSING GATE**  
  
 - Lanes are removed when vehiles have an appointment cancelled or postponed.  
  
**FIXES**  
  
 > **Create appointment**  
  
 > - Advisors availability panel is now shown updated after clickin on _Create_ (appointment).  
  
---  
 

# Versión 17.08.02
   
**NEW FEATURES**    

> - Add motor letters on vehicle information, in customer card and appointment summary. 

>**APPOINTMENT**

> - Allow to add dealer packages with external services and other charges.

**IMPROVEMENTS**

>**LOGISTIC**

> - Only appears on logistic screen vehicles that had arrived through the barrier.
> - Autorefresh vehicles pending to retire when the screen is active again, after mobile unlock, change of tab in browser. 
> - Inform other logistic when a vehicle is already retired. 
> - From now all vehicles pending to retire, independently of order status or arrival date, will appear. 
> - Add reception location and reception date, highlighting with color vehicles from previous days. 

>**LANE STATUS**

> - Change icon trash with a tick, to avoid misunderstanding. 
> - Add reception location and arrival to workshop date, highlighting with color vehicles from previous days. 
 
---   
# Versión 17.07.24   
  
**NEW FEATURES**    

> **CUSTOMER**

> - Visualize customer address during the appointment.
> - Modify customer hints during the appointment and in opportunity card.
  
> **REPLACEMENT VEHICLES**

> - Replacement vehicles reservation follow up. 
> - Replacement vehicles delivery, with digital signature and send email to the customer with the contract. 
> - New layout available to design replacement vehicle contract email. 
> - New layout to define contract clauses, visible in both, during the delivery in the web and in the signed contract. 
  
> **CUSTOMER MANAGER**    

> - Visualize replacement vehicle reservation.
> - Discard a vehicle without appointment.      
  
> **APPOINTMENT MANAGEMENT**    

> - Visualize the list of appointments created from the customer portal to know which are to be reviewed.    
 
**IMPROVEMENTS**     

>-  New component for appointment reservation in advisers agenda during the process.

**FIXES**     

> - Fixed error related with timezone which result was a wrong availability or availability was not shown.  
> - Internal app logs improved to have more traceability of the system.
> - Users with General job in the workshop ae not going to be shown as available for appointments..
    
---   

# Versión 17.06.14   
  
**FIXES**    
  
 - When looking for jobs by workshops they were sought in all workshops. Now we will only find the jobs of the workshop to which they will be added.

 ---   
 
# Version 17.04.18    
  
**NEW FEATURES**  
  
 > **Appointment creation**  
  
 > - Management permission for replacement vehicles in the mobility manager form and in the rate groups and replacements vehicles.  
 > - Active Selling for Ducati.  
 > - Changing the configuration won't overwrite the target's config file in the next deployment. Service will take the default file in case there is no configuration file.    
  
**FIXES**  
  
> **Appointment creation**    

 > - **Adviser appointment reservation:**   
 > - Adviser appointments were not working in UTC time format and their availability was being shown according to time difference frmo the UTC time.   
 > - Appointment time is check so that it matches the time selected in the _Appointment creation_.      
    
---   
   
# Version 17.04.11   
  
**NEW FEATURES**  
      
 > ### Appointment creation    
 >> - Add remarks to jobs.  
 >> - Add remarks to the order.   
 >> - Show the number of the order in the reservation form for replacement vehicle.    
  
---      
  
# Version 17.03.13  
  
**NEW FEATURES**
 
 > **Customer card**  
  
 >> - Visualize all PPSO and Active Selling offers.   
 >> -  Visualize last depositary.  
 
 > **Workshop appointment**  
    
 >> - Visualize ElsaR campaigns during the appointment creation process.  
  
  
  
 > **PPSO packages**
  
 >> - Visualize PPSO package details.    
 
 > **Add jobs **  
  
 >> - Add jobs without established positions.  
  
 > **User permissions**  
  
 >> - Prevent users without the rights permissions to create an appoinment.
  
 ---
  
# Version 17.01.26    
  
**NEW FEATURES**  
  
 > **Customer manager**
    
 >> - Search box for _third party_ and _number plate_.  

---   
  

# Version 17.01.23      
  
**NEW FEATURES**  
  
 > **Customer manager **   
  
 >> **Notifications**
  
>>> - Notify that a customer wihtout date has arrived.
  
      
 
 > **Workshop logistics**  
  
 >> - Visulize already receptioned vehicles waiting to be led to the workshop to be attended in the workshop.     
 >> - Visualize that a vehicle has been moved from the queue (green sign) so that we can control the remaining ones.    
       
  
**IMPROVEMENTS**   
  
 
 > - Visualize price according to the currency defined in the enterprise.    
 > - Show kilometers of the vehicle in the history of jobs.  
  

  
---   
   
  
# Version 16.12.22   
  
**NEW FEATURES**  
  
 > **Rates group**  
  
 >> - Set price to replacement vehicles for rental.  
 >> - Manage group and rates of replacements vehicles.  
  
 > **Create appointment**  
  
 >> - Show price for replacement vehicles for rental.    
  
 > **Customer manager ** 
  
 >> - Visualize notifications when a customer without an appoinment has arrived.      
  
**IMPROVEMENTS**    

  > - Text text "El cliente dice que" ("customers says that..." is added for free jobs.  
  

 
---  
    
# Version 16.11.21  
  
**NEW FEATURES**
  
 
 > **Customer manager** 
  
 >> - Notify the recepcionist of the arrival of a customer.
 >> - Notify the recepcionist of a vehicle that is already at service reception.
 >> - Notify other user of the customer manager that a customer has already arrived.
    
 > **Actives Search**  
  
 >> - Visualize market campaigns both _currently being applied_ and _pending to be scheduled_..    
  
 > **Appointment creation**  
  
 >> **Fixes**  
  
 >>> - Appointments could not be created if the remarks field were to big.  

---      
  
  
# Version 16.31.10    
  
**NEW FEATURES**   
  
### General improvement  
  
 > - Calculation process performance increases for the target _Next maintenances_.
   
### Appointment creation    
  
 > **New features**
  
 >> - Appointment creation for _darft_ vehicles.     
 >> - An appointment confirmation email is sent to our customer.  
 >> - Layouts are customized for the appoinment reminders by brand.
  
> **Fix**  
  
 >> - Creating an appointment ended in error when there weren't engine codes.
  
### Customer profile    
  
 > **New features**
  
 >> - Check all the contact information of a customer.
 >> - Edit the contact information of a customer. 
 >> - Select how the customer wants to be contacted for appointments reminder.    

---  

  
  
# Version 16.10.05
  
**APPOINTMENT CREATION**  

 
> **Improvements**    
  
> - _Save_ button is relabeled by _Create_ to clarify the start and end of the appointment creation process.    
> - Appointment's availability adjusts automatically after modifiyng the period of a previous appointment.  

---   
  

# Version 16.09.26    
  
**NEW FEATURES**  
  
 - Search for vehicles accepts inserting the name of a customer.      
 - Notes related to a certain customer are now accesible from the customer's card (bell icon).
  
 
**Fixes**  
  
 - Added language to component _remoteselect2_.  


  
 **CUSTOMER MANAGER**  
   
 - Visualize the customer requests a taxi.  
 - Visualize the active reception request for a customer.
  
**APPOINMENT CREATION**  
  
  - Note that the customer requests a taxi.   
  - Note that the customer accepted active reception.     

**Improvements**  
  
 - New design for the summary of the appoinment to improve readability.   
  
---    
 
  
# Version 16.09.07  
  
**IMPROVEMENTS**   
 
 - Tooltips appear in all internet browsers.
  
**APPOINMENT CREATION**    
  
>**New features**  
>  
>  - Campaigns are shown if my dealer is responsible of them.
  
>**Improvements**
  
 > - Damages can be created with a text name longer thatn 100 characters (text is truncated).  
 > - Delete importer packages from the Dealer after adding it (Market packages).
> - Names of customer are truncated when they are too long.
  
---  

  
# Version 16.09.02  
  
**CUSTOMER MANAGER**    
  
**New features**  
> - Note which vehicle has come to the workshop (appointment).  
> - Check next vehicles/appointments for today.     
  
 
    
  **APPOINMENT CREATION**      
  
>*New features**
  
  >  - Edit the initially estimated time for a job.  
  >  - Segment the time for jobs.  

**Improvements**    
  
 > **Vehicles under campaigns**
  
   >>  - Current filter selection is kept during navigatin between pages.  
    

---  
  
 
  
  
# Version 16.08.16   
  
**NEW FEATURES**   
  
 - **Campaigns**  
>  
> - Add available campaigns for a VIN during the appointment creation process.
> - Navigation between an opened opportunity and the list of campaigns keep the previous filter criteria.    
    
 
**IMPROVEMENTS**   
  
- **Opportunities on VIN's**  
> - Vehicles sold by our agents will not be shwon as opportunities. 
 



  
  
  
---  
  
    
# Version 16.08.10   
  
**NEW FEATURES**   
  
 - **Campaigns**  
>  
>   - Select brand and campaigns to visualize related vehicles (VIN).   
> - Add available campaigns for a VIN during the appointment creation process.
   
    
 - **Packages:**   
  
> - Visualize and add packages from the Importer and the Dealer in order to give a price to customers.
  

  
**IMPROVEMENTS**   
  
- **Opportunities on VIN's**  
> - Vehicles sold by our agents will not be shwon as opportunities. 
  
 - **Packages**    
> - Packages will be shown depending on the brand of the vehicle. Thos vehicles whose VIN does not exist in the Importer will be also shown.
  
 - **Mean of contact**  
> -  The default mean of contact will be set according to the mean of contact active for every market.



---   
  
  
   

#Version 16.07.21  
  
 **NEW FEATURES**  
  
  - Add packages and offers for any brand during the appointment creation.
  
- Add dealer packages during the appointment creation process.
  

**IMPROVEMENTS**  

  - Wider range of dates (+15 days) to assign to an appoinment.   

---    


#Version 16.07.08    

**NEW FEATURES**  

 - Note that a damage os repetitive, during the appointment creation process.  
  
---  
     

#Version Iteration 16.06.29    
  

**NEW FEATURES**  

         
 - Create an appointment for one of your workshops.  
 - Check the works summary always accesible from Active Search and the Appointment`s summary.  
  
---  


  
#Version 16.05.05  

**NEW FEATURES**  

  - Check already-made campaigns.  
  
**IMPROVEMENTS**  

 - Modal information about cusomter's feedback.
 - Number plate seach is enhaced.

---  
  
#Version 16.03.23   


**NEW FEATURES**    

- Selector to change the enterprise.

**IMPROVEMENTS**  

 - User actions are managed in the active window tab.  

**FIXES**  
  
 - Exchange is switched off as reminder system.

---  

#Version 16.03.07
  
**NEW FEATURES**   
 
- List of vehicles under campaigns.    
- Feedback for offered campaigns.  
- Show when a maintenance service is already scheduled to avoid offering it again to the customer.  


---  



#Version 16.02.23     
 **NEW FEATURES**   

 - _Requires_ registered in Mobile Workshop are now shown in the opportunity card. 
 - The target of _Requires_ only shows the _pending_ requires.
 - A dashboard shows a card with the number of opportunities for today.
    

**IMPROVEMENTS**  
 
 - Remarks can only be added after selecting a feedback.
  
 
---  

#Version 16.02.11  

**NEW FEATURES**  

   - Different configurations can be applied according to user market or working brand.   
   - List for Requires (Mobile Workshop) is shown in the left menu.

**IMPROVEMENTS**    

 - Target of spark plugs applies only to gas vehicles.  
 - The configuration of the maintenance service depends on the engine code.
    
---  

#Version 16.01.25  
  
- Target of Warranty expiration.  
- Target of spark-plugs includes configurations for engine codes.
- Feedback for more than one maintenance services at once and for incoming customer call.
- Access to Opportunity enterprises in different environments
     
**IMPROVEMENTS**  
  
 - Vehicles with timing chain are excluded from Target of timing belt.    
 - Date for _Next maintenances_ updates after noting new kilometers in the feedback window.
 - New rejection reasons included: "Maintenance will be made by another official service".

---

#Version 16.11.01
  
  

 **NEW FEATURES**    
 
 - Access to opportunities's list of _Reminder_ feedback.
 - Target of call for Brakes fluid.  
 - Reason of rejection feedback is now tabulated. 
    

 **IMPROVEMENTS**  

 - Reminder showed in Outlook gives information of the Dealer owning the opportunity.
 
---  

#Version 15.12.18  

**NEW FEATURES**  

 - Target of call for next timing-belt change.  
 - Target of call for spark-plug change.  
   
**IMPROVEMENTS**      
   
 - The customer card shows information about the _Last inspection date_ and _Estimated date_ for the maintenance plan.

---  


#Version 15.12.02     
**NEW FEATURES**    

- Navigation for opportunties.   
- _Call me later_ feedback is shown again as opportunity.  
- Open an opportunity from the plate-number search box.  
- Target for next maintenances   
   
  
---

#Version 15.11.20  
  
**NEW FEATURES**    

 - Opportunities include fleet vehicles whose holder is not a fleet nor a dealer. 
 - Access to Help User Documentation.  
   
  
**IMPROVEMENTS**  
  
 - User interface and UX  

---  

  
#Version 15.11.04  
**OPPORTUNITY**

**NEW FEATURES**  
  
   -  Automatic check for customers with a maintenance contract or warranty extension contract.  
  - Register for call a customer in a certain date.  
  - Number of opportunities are displayed visually.  
  - Manufacturer campaigns are shown for each vehicle.    
  - Kilometers, kilometers estimation and first maintenance are shown.  
  - Feedback for kilometers informed by the customer.  
  - Call frequency is managed for clients that haven't picked up the phone.  
  - First maintenance only shows related brands.   

**IMPROVEMENTS**    

- Estimations discards the notation of the kilometer marke corresponding to the first month of the vehicle.  
 

---  

#Version 15.10.27    

**NEW FEATURES**   
 
- 22 months is established as minimum time to be included in Opportunity.  
- _Call me later_ feedback.  
- VIN is shown next to the information of a vehicle.  
 
  
---    




   
#Version 15.10.07  
**NEW FEATURES**  
  
 - Show the owner of the vehicle.  
 - _First Maintenance_ mail contact for clients.  
 - Show information about warranties.  
 - Prioritize the _Opportunities_.  
  


**IMPROVEMENTS**  
  
- Rent-a-car clients are excluded from _Opportunity_ list.  
- Transfer vehicles client´s are excluded from _Opportunity_ list.    

---  


#Version 15.09.11    

**NEW FEATURES**  

- _Target_ for customers to be contacted by telephone.  
- History of contacts made with a customer.    
- Interface to fill in reminders and positive/negative feedback.


