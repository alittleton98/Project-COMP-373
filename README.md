# Project COMP-373

#### Adam Delaney/Andrew Littleton

#

## Requirements
Design and implement a facility management system complete with user management, facility maintenace management, and internal faciltiy management. Written in Java

### Project 1: Facility Management System Design and Implementation

Initial design and implementation for the management system.  
Designed with 3 Packages:  

1. facility - The internal members and methods of each Facility and the Facility interface
2. maintenance - The members and methods requried to make maintenance requests and schedule maintenace for each facility
3. use - The members and methods required for making and managing facility usage and users

### Project 2: Object Wiring with Spring Framework

Setup new classpath and spring container configuration/dependency relationships through xml configuration. Used ApplicationContext mechanism.

### Project 3: Bridge/Observer Implementation

Bridge Implementation added by abstracting maintenance and use interfaces to the FacilityOperations class.  
FacilityOperations is used by Facility and Client to perform and maintenace or use management methods rather than having to call them separately.
  
Observer implementation added by having the Facility class act as observer to the newly created FacilityOperations class. FacilityOperations can create things like MaintenanceRequests for certain Facilities, and individual Facilities should be observing FacilityOperations and then be updated automatically to include the newly created MaintenanceRequests, Inspections, Uses, etc for their specific Facility.  

### Project 4: Visitor/Builder Implementation

Visitor design implemented using the Facility Manager and Facility Operations Manager. Visitor object will visit the class, the class will accept the visit and return true upon acceptance, then the vistor will then "audit()" the class (functionality undecided, but action performed). Visitor has visit() function defined for each 

*UML Updated to reflect changes*
