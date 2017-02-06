# Cloud-Computing-and-Big-Data-CS499-Assignment2

The entities created are: blog, tag, and entry.

blog: 
    field1: name (String)	field2: handle (String)

	relationship: many-to-one w/ user with "login" field
	relationship: one-to-many w/ entry with "login" field

tag:
    field: name (String)
	
	relationship: many-to-many w/ entry

entry:
    field1: title (String)	field2: content	(CLOB)	field3: date (ZoneDateTime)

    	relationship: many-to-one w/ blog with "name" field
	relationship: many-to-many w/ tag with "name" field
