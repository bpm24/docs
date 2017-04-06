The connector is one of the main components of the bpm engine. It plays 
the role of a handler, allowing to complete such actions as integrating 
with different CRM systems, importing and exporting data into the database, 
as well as interacting with a number of external services etc.

###Structure
```
{
    id: '',      
    name: '',
    description: '',
    type: '',       
    code: {
        before: '',
        after: '',
        script: ''
    },       
    params: {},    
    context: [],
    global: [],
    previousConnectors: [],
    nextConnectors: []
}
```

The connector logic is written in JavaScript. The connector has 3 sections 
for the code – Before, After and the main Script section. If you intend 
to develop your own solution, it is advisable to write the connector code 
in the Script section. However, if you would like to override a method or 
create additional handlers, use the sections Before and After.

