All types and type members have an accessibility level. The accessibility level controls whether they can be used from other code in your [[Assembly|assembly]] or other assemblies.
The following access modifiers are used to specify the accessibility of a type or member when you declare it:
- **public**: The type or member can be accessed by any other code in the same assembly or another assembly that references it. The accessibility level of public members of a type is controlled by the accessibility level of the type itself.
- **private**: The type or member can be accessed only by code in the same class or struct.
- **protected**: The type or member can be accessed only by code in the same class, or in a class that is derived from that class.
- **internal**: The type or member can be accessed by any code in the same [[Assembly|assembly]], but not from another assembly. In other words, internal types or members can be accessed from code that is part of the same compilation.
- **protected internal**: The type or member can be accessed by any code in the assembly in which it's declared, or from within a derived class in another assembly.
- **private protected**: The type or member can be accessed by types derived from the class that are declared within its containing assembly.
