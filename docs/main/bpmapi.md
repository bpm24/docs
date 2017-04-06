A bpm object is accessible in the global connector visibility area. You 
may use this object in the pre and post section of the connector. The 
object provides a basic system api for processes, which allows to manage 
process behaviour and create new connectors.

##Properties

####bpm.workspace
Workspace identifier

####bpm.contextId 
Context identifier

####bpm.contextInd
Context branch index

####bpm.process
Object containing process information

####bpm.connector
Object describing current connector

####bpm.ctxTree
Context branch not intended for editing (data editing does not affect the context)

####bpm.ctx
Current branch context, intended for working with the context

####bpm.global
Global process context, includes steps sections and variables, may change at any step when the process is running

####bpm.previous
Array containing identifiers of executed connectors in the current branch


##Methods

!!! warning "Please note"
    All methods return the object Promise

###Working with the context
####bpm.save()
This method allows to save changes in the branch context, global context and variables.

####bpm.getFromContext(deepString)
Method for obtaining context data based on the identifier. Obligatory prefixes:
```global``` или ```context```

| Name | Type | Description |
| --- | --- | --- |
| deepString | <code>String</code> |  Example: ```context.58b884ac27218c2441d94f2b.param``` |

###Working with connectors
####bpm.getConnectorById(id)
Method for obtaining the connector based on its identifier

| Name | Type | Description |
| --- | --- | --- |
| id | <code>String</code> | Connector identifier |

####bpm.setNextConnectors(connectors)
Method overriding identifiers of connectors that will be requested after handling the current connector

| Name | Type | Description |
| --- | --- | --- |
| connectors | <code>Array</code> | Array of connector identifiers |

####bpm.stopTimers()
Method allowing to cancel the handling of timers tied in with the step

####bpm.removeTimers()
Method allowing to delete the timers tied in with the step

###Working with the Process

####bpm.stopProcess()
Method to abort the process
 
###Working with the Storage

####bpm.storage.get(name, data)
This method is used to select documents from the Storage

| Name | Type | Description |
| --- | --- | --- |
| name | <code>String</code> | Storage name |
| data | <code>Object</code> | [Storage protocol](/storage/protocol) |

####bpm.storage.create(name, data)
This method is used to create a document in the Storage

| Name | Type | Description |
| --- | --- | --- |
| name | <code>String</code> | Storage name |
| data | <code>Object</code> | [Storage protocol](/storage/protocol) |

####bpm.storage.update(name, data)
This method is used to update a document in the Storage

| Name | Type | Description |
| --- | --- | --- |
| name | <code>String</code> | Storage name |
| data | <code>Object</code> | [Storage protocol](/storage/protocol) |

####bpm.storage.remove(name, data)
This method is used to delete documents from the Storage

| Name | Type | Description |
| --- | --- | --- |
| name | <code>String</code> | Storage name |
| data | <code>Object</code> | [Storage protocol](/storage/protocol) |

####bpm.storage.count(name, data)
This method is used to count the number of documents in the Storage

| Name | Type | Description |
| --- | --- | --- |
| name | <code>String</code> | Storage name |
| data | <code>Object</code> | [Storage protocol](/storage/protocol) |