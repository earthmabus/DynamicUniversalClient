# DynamicUniversalClient
If you ever wanted to truly understand, manage, and control your CORBA infrastructure, then this is the application for you!

It is the SoapUI equivalent for CORBA -- acquire CORBA objects, invoke requests against them, visualize return values, and a whole lot more!

This project has been divided into several applications:
* DynamicUniversalClient (DUC) - This application is a UI that provides the ability to acquire CORBA objects, inspect them, invoke requests against them, visualize return values, and a whole lot more!
* CIM - This application is an alternative to CORBA's Interface Repository.  The model is accessible via CORBA and is easy to understand and around.  This application is utilized by the DUC to acquire the IDL for datatypes encountered during runtime.
* InterfaceRepositoryToCIM - This application is used to transfer the contents of an Interface Repository into a CIM.  An alternative approach to populating the CIM would be to build an IDL parser.
* ObjectWrapper (OW) - This application allows any CORBA object encountered to be decorated with another CORBA object.  The decorator intercepts all incoming requests to the CORBA object so that it can be analyzed.
* ObjectWrapperDataAndStatisticsGatherer (OWDSG) - This application collects data and generate statistics for wrapped CORBA objects.
