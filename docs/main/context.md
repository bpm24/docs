The main purpose of the context is driving process data from one connector 
to the other. One context may have several process branches, which means 
that the connectors may generate new context branches.

When a process is created, a new context is set up at the same time. 
The context is filled with sections containing connector parameters. 
Default parameter value is null. After each connector handling, the 
context is saved and cloned for the next connector, including saved 
values, which allows for data accumulation.

Example of a created context:

```{
	«stepId»: {
		«propertyName»: null
	}
}```

The context contains connector sections and a data section, where random 
values may be written.

The context does not provide for creating random sections.