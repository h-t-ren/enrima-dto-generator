enrima-dto-generator
====================

Develepment environments:
------------------------

* JDK 1.6 or above
* Maven 3.0.0 or above
* Git (optional)

Download the project:
------------------------

* git clone git://github.com/h-t-ren/enrima-dto-generator.git
* or https://github.com/h-t-ren/enrima-dto-generator and click "zip" button 

Compile and install:
------------------------

* cd enrima-dto-generator
* mvn clean install



Importance files:
====================

* Tree structure:

<pre>
├── pom.xml
├── README.md
├── src
│   └── wsdl
│       ├── enrima-gui.wsdl
│       └── enrima-gui.xsd
└── target
    ├── jaxws
    │   ├── stale
    │   └── wsimport
    │       └── java
    │           └── eu
    │               └── enrima
    │                   └── gui
    │                       └── dto
    │                           ├── Building.java
    │                           ├── Demand.java
    │                           ├── EnergyMarket.java
    │                           ├── EnergyType.java
    │                           ├── EnrimaResource.java
    │                           ├── EnrimaResourceService.java
    │                           ├── EnvironmentParameter.java
    │                           ├── GetEnvironmentParametersRequest.java
    │                           ├── GetEnvironmentParametersResponse.java
    │                           ├── HeatSystem.java
    │                           ├── HVACSystem.java
    │                           ├── InternalBuildingParameter.java
    │                           ├── MarketPrice.java
    │                           ├── ObjectFactory.java
    │                           ├── package-info.java
    │                           └── Results.java

</pre>


* Dependence management and deploy file
 - pom.xml

* Source files:
   
 - src/enrima-gui.xsd (the schema)
 - src/enrima-gui.wsdl (include schema and operations/messages/binding/port definition)

* Generated files (after running the command: mvn clean install ):
 - target/jaxws/wsimport/java/en/enrima/gui/dto/*.java
