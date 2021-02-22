# DynamicUniversalClient
If you ever wanted to truly understand, manage, control, debug, test, etc. your CORBA infrastructure, then this is the application for you!  

It is the SoapUI equivalent for CORBA.  Using the application, you'll be able to acquire CORBA objects, invoke requests against them, visualize return values, and a whole lot more!  Here's a [simple video of the Dynamic Universal Client](https://youtu.be/EXURgWWZqgc) in action!

This project has been divided into several applications:
* **DynamicUniversalClient (DUC)** - This application is a UI that provides users the ability to acquire CORBA objects, inspect them, invoke requests against them, visualize return values, and a whole lot more!
* **CIM** - This application is an alternative to CORBA's Interface Repository. The model presents itself through a set of CORBA interfaces, is easy to understand, and can be utilize by other projects.  CIM is utilized by the DUC to acquire the IDL for datatypes encountered during runtime.
* **InterfaceRepositoryToCIM** - This application is used to transfer the contents of an Interface Repository into a CIM.  (Note: An alternative approach to populating the CIM would be to rewrite this into an IDL parser.)
* **ObjectWrapper (OW)** - This application wraps specified CORBA objects (using the Decorator design pattern).  The OW intercepts and analyzes all incoming requests to wrapped CORBA objects.
* **ObjectWrapperDataAndStatisticsGatherer (OWDSG)** - This application collects data and generate statistics for wrapped CORBA objects.
