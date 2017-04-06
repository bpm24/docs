The storage is intended for storing various data. The storage is in fact 
an HTTP protocol-based add-on to the direct access to the database 
(we use MongoDB).

We recommend to use the storage for keeping permanent data, such as users, 
groups, goods and uploads from external systems. The storage may also be 
used for connector settings, conditions, time values etc.

***Storage structure***
```
{
    id: '',
    name: '',
    ACL: {
        create: [],
        read: [],
        update: [],
        delete: []
    }
}
```


***Document structure in the storage***

We do not impose any restrictions on the structure of your data. You 
determine it yourself.

