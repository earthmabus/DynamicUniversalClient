# DynamicUniversalClient
This is the ultimate suite of tools to understand, manage, control, debug, and test your CORBA infrastructure.  If interested, please contact me at **earthmabus@hotmail.com**.

This project has been divided into several applications:
* **DynamicUniversalClient (DUC)** - This application is a UI that provides users the ability to acquire CORBA objects,  invoke requests against them, visualize return values, and a whole lot more!  It is the SoapUI equivalent for CORBA.  Here's a **[simple video of the Dynamic Universal Client](https://youtu.be/EXURgWWZqgc)** in action!
* **ObjectWrapper (OW)** - This application is used to capture all of the information for all of the requests made against a specified set of CORBA objects.  Users can view the parameters, return value, and/or exceptions for all requests through a UI or via MongoDB queries.  (This application is similar to AWS CloudTrail.)
* **CIM** - This application is an alternative to CORBA's Interface Repository. The model presents itself through a set of CORBA interfaces, is easy to understand, and can be utilize by other projects.  CIM is utilized by the DUC to acquire the IDL for datatypes encountered during runtime.
