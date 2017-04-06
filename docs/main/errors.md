#Error codes:
All returned errors have the following form:

```
{ 
    error_code: <int>,
    error_message: <string>,
    more_info: <string>
}
```

##Code description

####500
```
{ 
    error_code: 500,
    error_message: 'Internal error',
    more_info: 'https://bpm24.cloud/docs/main/errors/#500'
}
```

Internal error, error data logged additionally. 


####600
```
{ 
    error_code: 600,
    error_message: 'Workspace not found',
    more_info: 'https://bpm24.cloud/docs/main/errors/#600'
}
```
Error occurs when a non-existent workspace is addressed.

####601
```
{ 
    error_code: 601,
    error_message: 'Workspace schema isn't valid',
    more_info: 'https://bpm24.cloud/docs/main/errors/#601'
}
```
Error occurs when an invalid scheme is transmitted or when an error has 
occurred in the type of transmitted data while saving or updating. 

####602
```
{ 
    error_code: 602,
    error_message: 'Workspace is already exist',
    more_info: 'https://bpm24.cloud/docs/main/errors/#602'
}
```
Error occurs if this workspace already exists.

####603
```
{ 
    error_code: 603,
    error_message: 'Name of workspace is incorrect',
    more_info: 'https://bpm24.cloud/docs/main/errors/#603'
}
```
Error occurs if workspace name in the query has a wrong format or is empty.

####604
```
{ 
    error_code: 604,
    error_message: 'Storage schema is invalid',
    more_info: 'https://bpm24.cloud/docs/main/errors/#604'
}
```
Error occurs if an invalid scheme is transmitted while creating the storage 
or if an error has occurred in the type of transmitted data while saving or updating.

####605
```
{ 
    error_code: 605,
    error_message: 'ACL of storage isn't valid',
    more_info: 'https://bpm24.cloud/docs/main/errors/#605'
}
```
Invalid ACL transmitted in the query.

####606
```
{ 
    error_code: 606,
    error_message: 'Exceeded max number of storages',
    more_info: 'https://bpm24.cloud/docs/main/errors/#606'
}
```
Maximum number of storages reached.

####607
```
{ 
    error_code: 607,
    error_message: 'Name of storage is already exist',
    more_info: 'https://bpm24.cloud/docs/main/errors/#607'
}
```
A storage with this name already exists.

####608
```
{ 
    error_code: 608,
    error_message: 'Name of storage must be more 3 chars',
    more_info: 'https://bpm24.cloud/docs/main/errors/#608'
}
```
Storage name cannot be less than 3 symbols.

####609
```
{ 
    error_code: 609,
    error_message: 'Name of storage not found',
    more_info: 'https://bpm24.cloud/docs/main/errors/#609'
}
```
Error occurs when a non-existent storage is requested.

####610
```
{ 
    error_code: 610,
    error_message: 'Id of storage isn't valid',
    more_info: 'https://bpm24.cloud/docs/main/errors/#610'
}
```
Invalid storage identifier transmitted.

####611
```
{ 
    error_code: 611,
    error_message: 'Index isn't valid',
    more_info: 'https://bpm24.cloud/docs/main/errors/#611'
}
```
Invalid index transmitted.

####612
```
{ 
    error_code: 612,
    error_message: 'Storage protocol isn't valid',
    more_info: 'https://bpm24.cloud/docs/main/errors/#612'
}
```
Invalid format transmitted for working with storage files.

####613
```
{ 
    error_code: 613,
    error_message: 'Process schema isn't valid',
    more_info: 'https://bpm24.cloud/docs/main/errors/#613'
}
```
Invalid process data transmitted or an error has occurred in the type of 
data transmitted.

####614
```
{ 
    error_code: 614,
    error_message: 'Title of process must be more than 3 chars',
    more_info: 'https://bpm24.cloud/docs/main/errors/#614'
}
```
Process name cannot be less than 3 symbols.

####615
```
{ 
    error_code: 615,
    error_message: 'Name of variable is invalid',
    more_info: 'https://bpm24.cloud/docs/main/errors/#615'
}
```
Variable name empty or invalid.

####616
```
{ 
    error_code: 616,
    error_message: 'Unknown variable type',
    more_info: 'https://bpm24.cloud/docs/main/errors/#616'
}
```
Unknown variable type transmitted.

####617
```
{ 
    error_code: 617,
    error_message: 'Id of ACL is invalid',
    more_info: 'https://bpm24.cloud/docs/main/errors/#617'
}
```
Invalid ACL transmitted.

####618
```
{ 
    error_code: 618,
    error_message: 'Process not found',
    more_info: 'https://bpm24.cloud/docs/main/errors/#618'
}
```
Non-existent or remote process requested.

####619
```
{ 
    error_code: 619,
    error_message: 'Process is running, can't edit',
    more_info: 'https://bpm24.cloud/docs/main/errors/#619'
}
```
This error occurs when updating a running process is attempted.

####620
```
{ 
    error_code: 620,
    error_message: 'Id of process isn't valid',
    more_info: 'https://bpm24.cloud/docs/main/errors/#620'
}
```
Invalid process identifier transmitted.

####621
```
{ 
    error_code: 621,
    error_message: 'Schema of connector isn't valid',
    more_info: 'https://bpm24.cloud/docs/main/errors/#621'
}
```
Invalid connector format transmitted or an error has occurred in connector type.

####622
```
{ 
    error_code: 622,
    error_message: 'Unknown connector type',
    more_info: 'https://bpm24.cloud/docs/main/errors/#622'
}
```
Unknown connector type transmitted.

####623
```
{ 
    error_code: 623,
    error_message: 'Missing <some text>',
    more_info: 'https://bpm24.cloud/docs/main/errors/#623'
}
```
Error occurs at connector validation and indicates that an obligatory 
section in connector parameters has been omitted.

####624
```
{ 
    error_code: 624,
    error_message: 'Invalid type of connector',
    more_info: 'https://bpm24.cloud/docs/main/errors/#624'
}
```
Error occurs when trying to create a “start” or “stop” type connector.

####625
```
{ 
    error_code: 625,
    error_message: '<some text>',
    more_info: 'https://bpm24.cloud/docs/main/errors/#625'
}
```
Error occurs if the user handler for connector parameters returns an 
error at validation. Error text is set by the user in the handler.

####626
```
{ 
    error_code: 626,
    error_message: 'Id of connector isn't valid',
    more_info: 'https://bpm24.cloud/docs/main/errors/#626'
}
```
Invalid connector identifier transmitted.

####627
```
{ 
    error_code: 627,
    error_message: 'Connector not found',
    more_info: 'https://bpm24.cloud/docs/main/errors/#627'
}
```
Error occurs when a non-existent connector is addressed.

####628
```
{ 
    error_code: 628,
    error_message: 'Not equal types',
    more_info: 'https://bpm24.cloud/docs/main/errors/#628'
}
```
Error occurs at connector update if a type is transmitted that does not 
correspond to the initial type. 

####629
```
{ 
    error_code: 629,
    error_message: 'Use different ids',
    more_info: 'https://bpm24.cloud/docs/main/errors/#629'
}
```
Error occurs when the connector tries to connect to itself.

####630
```
{ 
    error_code: 630,
    error_message: 'Stop can't be parent',
    more_info: 'https://bpm24.cloud/docs/main/errors/#630'
}
```
Error occurs at attempt to create a connector with a “stop” type outbound 
connection.

####631
```
{ 
    error_code: 631,
    error_message: 'The timer may have only one child',
    more_info: 'https://bpm24.cloud/docs/main/errors/#631'
}
```
Error occurs if more than one child connector attempts to connect to the timer.

####632
```
{ 
    error_code: 632,
    error_message: 'Start can't have parent',
    more_info: 'https://bpm24.cloud/docs/main/errors/#632'
}
```
Error occurs at connection attempt when a “start” connector acts as a child connector.

####633
```
{ 
    error_code: 633,
    error_message: 'The timer may have only one parent',
    more_info: 'https://bpm24.cloud/docs/main/errors/#633'
}
```
Error occurs if more than one parent connector attempts to connect to the timer.

####634
```
{ 
    error_code: 634,
    error_message: 'Alias is already exist',
    more_info: 'https://bpm24.cloud/docs/main/errors/#634'
}
```
Error occurs if a connection between the connectors already exists.

####635
```
{ 
    error_code: 635,
    error_message: 'Alias not found',
    more_info: 'https://bpm24.cloud/docs/main/errors/#635'
}
```
Error occurs if a connection between the connectors has not been established.

####636
```
{ 
    error_code: 636,
    error_message: 'Alias allow only for task or case',
    more_info: 'https://bpm24.cloud/docs/main/errors/#636'
}
```
Connection name can only be established for steps of the following type: “case”, “task”. 

####637
```
{ 
    error_code: 637,
    error_message: 'Unknow result name',
    more_info: 'https://bpm24.cloud/docs/main/errors/#637'
}
```
Error occurs when creating connection name, if the branch for this name is not specified in the parameters of the “results” section.

####638
```
{ 
    error_code: 638,
    error_message: 'Id is already exist',
    more_info: 'https://bpm24.cloud/docs/main/errors/#638'
}
```
Error occurs when validating the “results” section for a “case” type step, 
if the child connector identifier is already contained in the array for this section.

####639
```
{ 
    error_code: 639,
    error_message: 'Schema of veriable isn't valid',
    more_info: 'https://bpm24.cloud/docs/main/errors/#639'
}
```
Error occurs if an invalid scheme is transmitted for the variable or if 
an error has occurred in the type of data transmitted.

####640
```
{ 
    error_code: 640,
    error_message: 'Variable is already exist',
    more_info: 'https://bpm24.cloud/docs/main/errors/#640'
}
```
Error occurs if an existing variable is created. 

####641
```
{ 
    error_code: 641,
    error_message: 'Value of string is incorrect',
    more_info: 'https://bpm24.cloud/docs/main/errors/#641'
}
```
Error occurs if an invalid line type is transmitted in the “value” section.

####642
```
{ 
    error_code: 642,
    error_message: 'Value of date is incorrect',
    more_info: 'https://bpm24.cloud/docs/main/errors/#642'
}
```
Error occurs if an invalid date type is transmitted in the “value” section.

####643
```
{ 
    error_code: 643,
    error_message: 'Variable isn't set',
    more_info: 'https://bpm24.cloud/docs/main/errors/#643'
}
```
Error occurs if no values for obligatory variables were transmitted in 
the request when creating the process.

####644
```
{ 
    error_code: 644,
    error_message: 'Variable has incorrect of type',
    more_info: 'https://bpm24.cloud/docs/main/errors/#644'
}
```
Error occurs if the transmitted variable has a different type at the time of process creation.

####645
```
{ 
    error_code: 645,
    error_message: 'Connector hasn't previous connectors',
    more_info: 'https://bpm24.cloud/docs/main/errors/#645'
}
```
Error occurs is the handled connector has no connection to the parent connector.

####646
```
{ 
    error_code: 646,
    error_message: 'Parent сonnector is not equal a current connector',
    more_info: 'https://bpm24.cloud/docs/main/errors/#646'
}
```
Error occurs if the connector to be handled has no connection to the executing connector.