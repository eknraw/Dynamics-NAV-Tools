# Dynamics NAV XMLPort Generator

## About 

Dynamics NAV Object generator that will dynamically create XMLPorts. 

This is a single Page Object (ID 79999) based on the Field virtual table.  

## Configuration

Filter on TableNo for single tables or a range.  If this is not set it will generate an XMLPort for every table in the database.

* __Export path for objects:__ Select folder you want object files placed in.
* __Starting Object ID:__ Object ID of first object, will increment for each additional object
* __XMLPort Field/Variable:__ XMLport will either be all SourceType Field or Text. If using Text type all variables, GET,INSERT,MODIFY code is generated for you. Import only for now. NOTE: You will have to cut/paste the primary key fields for Option strings above the GET statement. 
* __Filter on Selected Values:__ If selected it will use a SETSELECTIONFILTER and only generate code for the fields that are highlighted. 

* __Split Object Files:__ Unchecked all objects will be a in a single AllObjects.txt file.  Checked they will be split and named by an incrementing Object ID as specified in the "Starting Object ID". Example: XML50100.txt object name, "50100 SalesHeader_50100"

* __Field Seperator:__  Sets the FieldSeperator property.

* __Field Delimeter:__  Sets the FieldDelimeter property.

## Use

Click "Generate XMLPorts" and import object(s) text files into destination database.

