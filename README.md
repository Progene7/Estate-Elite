# Estate-Elite

Focus: In this activity the focus will be on ER/EER Modeling, Relational schema 
design and refinement (Normalization), implementing database (creating tables 
with constraints and inserting initial data necessary) and writing SQL/PL-SQL code 
for data entry, updates, generating reports, manipulation and enforcing certain 
complex constraints or rules. 

Domain description: 
We assume a Property Rental Agency (PRA) scenario where the PRA facilitates 
mediating between Owners of a properties and the Tenants, across multiple cities 
in India. Both Owner and Tenants are treated as the users of the system. There is 
a supper user (only one) who is the DBA. Some users are just Managers. DBA can 
add/delete/modify other users. Managers can add/modify/delete a property. Add 
details about which property is rented to which tenant etc. Some users can play 
both owner and tenant roles. That is, they may give their property for rent and 
may seek another property from others for rent. A property can be a residential 
property (independent-house/flat) or a commercial property (shop or 
warehouse). Each property has an ID which is unique. Each property has an
owner. A user has adharID, name, age, address(includes door#, Street, city, state 
and PIN code) and multiple phone numbers. All users will have login credentials. A
user as an owner can register a property he wants to give for rent. Once a 
property is given to a tenant, we capture that information. That means, we 
capture details like what is property is rented to which tenant, rent per month, 
start_date, end_date, yearly hike in rent(in %), agency commission, and other info 
as necessary. A property may not have a tenant if it is not rented. We also 
maintain the history of renting for a property. Every property is entered in to the 
system with the details like propertyID, owner, available from which date, 
available till what date, rent pm, %ge of annual hike in rent, total area(not null), 
plinth area(not null), number of bed-rooms(if residential), number of floors, year 
of construction (not null), locality, address, other facilities etc. A user when he 
uploads a property becomes owner. He can upload zero to many properties. A 
user when he takes a property for rent becomes tenant. He can be a tenant for 
zero to many properties. 

Functionality Expected:
1. Adding user to the database by DBA with necessary privileges.
2. Allowing DBA and Manager to add/delete/update any property record.
3. Allowing owner to add/delete/update his property record only.
4. Allowing Admin and Manager to add property-rent details after property is 
rented by a tenant.
5. Generate a report on rent history of a property.
6. To check list available properties for rent with in a given city/locality/price
range.
7. To check the status of a property based on property ID by all users.
8. A tenant can’t insert/delete/modify any data in any table. He can just look 
for available properties for rent.
