# DTDL-OPCUA-Information-Models-Mapping
Mapping of Information Models between DTDL and OPC UA.
This project is an implementation of the Digital Twins Definition Language(DTDL) model in OPC UA. It defines an open Information Model defining the main six classes: Interface, Telemetry, Property, Control, Relationship and Component, implemented by the DTDL model. This Information Model is based on the version 2 of the DTDL model.

# Overview
Industry 4.0 is featured by a continuously-evolving digital transformation. It aims to automate all the traditional industrial practices, and it hopes to do so by bringing as much of the equipment from the physical space into the virtual domain. And this is where Digital Twins come into play. Digital Twins emerged as an experimental tech-nology set to enable replication of elements, functions, operations and dynamics of physical systems into digital world, with better control at testing, analysis, prediction and hazard prevention for sensitive processes. Different organisations are currently working aiming to standardize Digital Twin definition, interoperability and how to interact with these Digital Twins. Microsoft is one of them. 
The DTDL was born as an open source initiative by Microsoft and it is already used in many commercial services offered by Microsoft like IoT Hub, IoT Central, and Azure Digital Twins.

You can explore custom OPC UA Information Model, using software such as [UAModeler](https://documentation.unified-automation.com/uamodeler/1.3.0/html/sec_introduction.html) from Unified Automation.The xml file in models folder can be easily imported in every OPC UA SDK allowing information model xml file to be imported. Through the ua file using the UAModeler software it is possible to generate [Template set](https://documentation.unified-automation.com/uamodeler/1.3.0/html/sec_projecttemplateset.html) for OPC UA Server SDK based on Unified Automation C++, OPC UA Server SDK based on Unified Automation ANSI C and OPC UA Client SDK based on Unified Automation .NET.

# Mapping
This table presents the match between the DTDL classes and the corresponding Object or Variable name in the OPC UA Information Model. 

| DTDL Class | OPC UA Information Model | OPC UA SubType |
| ------------- | ------------- | ------------- |
| Interface  | DTDLInterfaceType | BaseObjectType |
| Telemetry  | DTDLTelemetryType | BaseObjectType |
| Property  | DTDLPropertyType  | BaseVariableType |
| Command  | DTDLCommandType  | BaseObjectType |
| Relationship  | DTDLRelationshipType | BaseObjectType |
| Component  | DTDLComponentType  | BaseObjectType |

