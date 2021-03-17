| .NET | ASP .NET | ASP .NET Core |
| --- | --- | --- |
| .NET is a developer platform made up of tools, programming language, and libraries for building many different types of applications | ASP.NET is a .NET framework that extends the .NET platform with tools and libraries specifically for building web apps. | ASP.NET Core is the open-source and cross-platform version of ASP.NET. |
| __Things Included__: 1. The __C#, F#, and Visual Basic programming languages__ 2. __Base libraries__ for working with strings, dates, files/IO, and more 3. __Editors and tools__ for Windows, Linux, macOS, and Docker | __Things Included__: 1. __Base framework for processing web requests in C# or F#__ 2. __Web-page templating syntax__, known as Razor, for building dynamic web pages using C# 3. __Libraries for common web patterns__, such as Model View Controller (MVC) 4. __Authentication system__ that includes libraries, a database, and template pages for handling logins, including multi-factor authentication and external authentication with Google, Twitter, and more. 5. __Editor extensions__ to provide syntax highlighting, code completion, and other functionality specifically for developing web apps | You should use ASP.NET Core for all new applications. |


# Dynamic Pages using C#, HTML, CSS and Javascript

* Razor provides a syntax for creating dynamic web pages using HTML and C#.
* Your C# code is evaluated on the server and the resulting HTML content  is sent to the user.
* Code that executes client-side is written in Javascript.
* ASP.NET integrates with Javascript Frameworks and includes pre-configured templates for single page app (SPA) frameworks like React and Angular

# Back-end Code

* When using ASP.NET your back-end code, such as business logic and data access, is written using C#, F# or Visual Basic.
* Because ASP.NET extends .NET, you can use the large ecosystem of packages and libraries available to all. 

# .NET Artchitecture

* *C#* programs run on *.NET*, a virtual execution system called the *common language runtime (CLR)* and a set of class libraries.
* The *CLR* is the implemention by Microsoft of the *common language infrastructure (CLI)*, an International standard.
* The *CLI* is __the basis for creating execution and developement environments in which languages and libraries work together seamlessly.__
* Source code written C# is compiled into an [intermediate language (IL)](https://docs.microsoft.com/en-us/dotnet/standard/managed-code) that conforms to the CLI specification.

* The IL code and resources, such as bitmaps and strings, are stored in an assembly, typically with an extension of .dll. An assembly contains a manifest that provides information about the assembly's types, version, and culture.

* When the C# program is executed, the assembly is loaded into the CLR. The CLR performs Just-In-Time (JIT) compilation to convert the IL code to native machine instructions.
* The CLR provides other services related to automatic garbage collection, exception handling, and resource management.
* Code that's executed by the CLR is sometimes referred to as "managed code," in contrast to "unmanaged code," which is compiled into native machine language that targets a specific platform.

* Language interoperability is a key feature of .NET. IL code produced by the C# compiler conforms to the Common Type Specification (CTS). 
* IL code generated from C# can interact with code that was generated from the .NET versions of F#, Visual Basic, C++, or any of more than 20 other CTS-compliant languages. 
* A single assembly may contain multiple modules written in different .NET languages, and the types can reference each other as if they were written in the same language.

* In addition to the run time services, .NET also includes extensive libraries. These libraries support many different workloads. 
* They're organized into namespaces that provide a wide variety of useful functionality for everything from file input and output to string manipulation to XML parsing, to web application frameworks to Windows Forms controls. 
* The typical C# application uses the .NET class library extensively to handle common "plumbing" chores.



# .NET used to develop the following:

1. Console apps
2. Web apps, web APIs and microservices
3. Mobile apps
4. Desktop apps -> Windows WPF
5. Game Development
6. Machine Learning
7. Internet of Things
8. Cloud native applications
9. Serverless functions in the cloud
10. Windows services

# Cross Platform

## You can create .NET apps for many operating systems, including

* Windows
* macOS
* Linux
* Android
* iOS
* tvOS
* watchOS

## Supported processor architectures include:

* x64
* x86
* ARM32
* ARM64


# .NET is open source, using [MIT and Apache 2 licenses](https://github.com/dotnet/runtime/blob/master/LICENSE.TXT) and is a project of the [.NET Foundation](https://dotnetfoundation.org/)

# In order to understand the .NET you are aware of C# basics

## C# is a modern, object-oriented, component-oriented and type-safe programming language.

* C# enables developers to build many types of secure and robust applications that run in the .NET Eco system.
* Several C# features help create robust and durable applications.
* [Garbage collection](https://docs.microsoft.com/en-us/dotnet/standard/garbage-collection/) automatically reclaims memory occupied by unreachable unused objects.
* [Nullable types](https://docs.microsoft.com/en-us/dotnet/csharp/nullable-references) guard against variables that don't refer to allocated objects.
* [Exception handling](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/exceptions/) provides a structured and extensible approach to error detection and recovery.
* [Lambda expressions](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/operators/lambda-expressions) support functional programming techniques.
* [Language Integrated Query (LINQ)](https://docs.microsoft.com/en-us/dotnet/csharp/linq/) syntax creates a common pattern for working with data from any source.
* Language support for [asynchronous operations](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/async/) provides syntax for building distributed systems.
* C# has a [unified type system](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/types/).
* All C# types, including primitive data types such as *int* and *double*, inherit from a single root *object* type.
* Furthermore, C# supports both user-defined [reference types](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/reference-types) and [value types](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/value-types).
* C# allows dynamic allocation of memory for objects and in-line storage for lightweight structures.
* C# supports generic methods and types, which provide increased type safety and performance.
* C# provides iterators, which enable implementers of collection classes to define custom behaviors for client code.

* C# emphasizes *versioning* to ensure programs and libraries can evolve over time in compatible manner.
* Aspects of C#'s design that were directly influenced by versioning considerations include the seperate *virtual* and *override* modifiers, the rules for method overload resolution, and support for explicit interface member declarations.


# C# Data types

1. __Value types__
2. __Reference types__

## Value types are:

* __Simple types__
  * __Signed integral__ : ``` sbyte,short,int,long```
  * __Unsigner integral__ : ``` byte,ushort,uint,ulong```
  * __Unicode characters__ : ``` char ``` which represents a UTF-16 code unit
  * __IEEE binary floating-point__ : ``` float,double ```
  * __High-precision decimal floating point__ : ``` decimal ```
  * __Boolean__ : ``` bool ```, which represents Boolean values -- that are either ``` true ``` or ``` false ```
* __Enum types__
  * User-defined types of the form ``` enum E {...} ```. An ``` enum ``` type is a distinct type with named constants.
  * Every ``` enum ``` type has an underlying type, which must be one of the integral types.
  * The set of values of an ``` enum ``` type is the same as the set of values of underlying type.
* __Struct types__
  * User-defined types of the form ``` struct S {...} ```
* __Nullable value types__
  * Extension of all other value types with a ``` null ``` value
* __Tuple value types__
  * User defined types of the form ``` (T1, T2, ...) ```

## References types are:

* __Class types__
  * Ultimate base class of all other types: ``` object ```
  * __Unicode strings__ : ``` string ```, which represents a sequence of UTF-16 code units.
  * User-defined types of the form ``` class C {...} ```

* __Interface types__
  * User-defined types of the form ``` interface I {...} ```

* __Array types__
  * Single-dimensional, multi-dimensional, and jagged. For example: ``` int[], int[,] ```, and ``` int[][] ```

* __Delegate types__
  * User-defined types of the form ``` delegate int D {...} ```
