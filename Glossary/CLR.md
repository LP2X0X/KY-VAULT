- Common Language Runtime is the **run-time environment in the .NET Framework** that runs the codes and helps in making the development process easier by providing the various services.
- The code that runs under the Common Language Runtime is termed as the Managed Code.
- CLR provides the services and runtime environment to the [[CIL]] code. Internally CLR includes the [[JIT compiler|JIT (Just-In-Time) compiler]] which converts the MSIL code to machine code which further executed by CPU. CLR also uses the .NET Framework class libraries. Metadata provides information about the programming language, environment, version, and class libraries to the CLR by which CLR handles the MSIL code.
![[Working_CLR 1.jpg|center]]

- Main components of CLR: 
	- **Common Language Specification (CLS):** It is responsible for converting the different .NET programming language syntactical rules and regulations into CLR understandable format. Basically, it provides Language Interoperability. Language Interoperability means providing execution support to other programming languages also in .NET framework.
	- **Common Type System (CTS):** Every programming language has its own data type system, so CTS is responsible for understanding all the data type systems of .NET programming languages and converting them into CLR understandable format which will be a common format.
	- **Garbage Collector:** It is used to provide the _Automatic Memory Management_ feature. If there was no garbage collector, programmers would have to write the memory management codes which will be a kind of overhead on programmers.
	- **JIT (Just In Time Compiler):** It is responsible for converting the CIL (Common Intermediate Language) into machine code or native code using the Common Language Runtime environment.