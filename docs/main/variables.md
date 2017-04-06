Variables are intended to transmit conditions between connectors in the 
workflow context.

***Structure of the variable:***
```
{
    name: 'variable1',
    type: string|date,
    value: '',
    isRequired: true
}
```

!!! warning "Please note" 
    Do not use variables to record big data. Big data should be stored in 
    Storage. 

The list of variables that are going to be available in the context is 
set while modelling the process. At process start, all variables and their 
values are copied into the global context (into the data section). While 
the process is executed, the variable exists in singular form and does not 
depend on the context branch. Every step can override the value of the 
variable in the pre- and post-handling section, as well as in the step 
handler itself. When a variable is created, a type is set up for it, for 
initial type validation.

!!! warning "Please note" 
    While the process is active, the variable may be overridden with any 
    data. It is therefore necessary to check data type when the connector 
    accesses the variable, if required.