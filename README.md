### Legend

* ![NOT DONE](images/red.png)  - Not Done
* ![IN PROGRESS](images/yellow.png) - In Progress
* ![PENDING REVIEW](images/blue.png) - Pending Review
* ![DONE](images/green.png) - Done




# Go Design Documentation

#### 1. Introduction

#### 2. Concepts in Go

* [2.1 Domain](2/2.1.md) ![DONE](images/green.png)

* 2.2 Implementation ![NOT DONE](images/red.png)

#### 3. Getting Started

* [3.1 Setting up your development environment](3/3.1.md) ![DONE](images/green.png)

* [3.2 How to go about making changes to the codebase](3/3.2.md) ![DONE](images/green.png)

* [3.3 How to add a configuration migration](3/3.3.md) ![DONE](images/green.png)

* [3.4 How to add a database migration](3/3.4.md) ![DONE](images/green.png)



#### 4. Technology Stack

* 4.1 Plugins Architecture - OSGi ![NOT DONE](images/red.png)

* [4.2 Object Relation Mapping (ORM) - Hibernate & IBatis](4/4.2.md) ![DONE](images/green.png)
    * [4.2.1 Hibernate](4/4.2.md#421-hibernate) ![DONE](images/green.png)

    * [4.2.2 IBatis](422-ibatis) ![DONE](images/green.png)

* 4.3 Caching - EhCache ![NOT DONE](images/red.png)

* [4.4 Dependency Injection (DI) - Spring](4/4.4.md) ![DONE](images/green.png)

* 4.5 Model View Controller (MVC) ![NOT DONE](images/red.png)

    * 4.5.1 Models - Java ![NOT DONE](images/red.png)

    * 4.5.2 Controllers - Servlets & Rails ![NOT DONE](images/red.png)

    * 4.5.3 Views - Rails & Velocity ![NOT DONE](images/red.png)

* [4.6 User Interface (UI) - jQuery & Prototype, SCSS, HTML](4/4.6.md) ![DONE](images/green.png)

* 4.7 Build Tool - Buildr ![NOT DONE](images/red.png)

#### 5. Architecture of Go

* [5.1 Overview](5/5.1.md#overview) ![IN PROGRESS](images/green.png)

* [5.2 Go Server](5/5.2.md#go-server) ![DONE](images/green.png)

    * [5.2.1 Configuration Management](5/5.2.md#521-configuration-management) ![DONE](images/green.png)

        * [5.2.1.1 XSD & XML](5/5.2.md#5211-xsd--xml) ![DONE](images/green.png)

        * [5.2.1.2 Schema Migration](5/5.2.md#5212-schema-migration) ![DONE](images/green.png)

        * [5.2.1.3 Config Repository](5/5.2.md#5213-config-repository) ![DONE](images/green.png)

        * [5.2.1.4 Config Merge](5/5.2.md#5214-config-merge) ![DONE](images/green.png)

        * [5.2.1.5 Config Diff](5/5.2.md#5215-config-diff) ![DONE](images/green.png)

    * [5.2.2 Database Management](5/5.2.md#522-database-management) ![DONE](images/green.png)

        * [5.2.2.1 Schema](5/5.2.md#5221-schema) ![DONE](images/green.png)

        * [5.2.2.2 Migration - DBDeploy](5/5.2.md#5222-database-migrations) ![DONE](images/green.png)

        * [5.2.2.3 Backup](5/5.2.md#5223-backup) ![DONE](images/green.png)

    * [5.2.3 Material Update Sub System](5/5.2.md#523-material-update-sub-system-mdu) ![DONE](images/green.png)

        * [5.2.3.1 Material Fingerprint & Flyweights](5/5.2.md#5231-material-fingerprint--flyweights) ![NOT DONE](images/red.png)

        * [5.2.3.2 Supported Materials](5/5.2.md#5232-supported-materials) ![NOT DONE](images/red.png)

    * [5.2.4 Build Cause Production](5/5.2.md#524-build-cause-production) ![IN PROGRESS](images/yellow.png)

    * [5.2.5 Pipeline Scheduling](5/5.2.md#525-pipeline-scheduling) ![IN PROGRESS](images/yellow.png)

    * [5.2.6 Work Assignment](5/5.2.md#526-work-assignment) ![NOT DONE](images/red.png)

        * [5.2.6.1 Resource & Environment Mapping](5/5.2.md#5261-resource--environment-mapping) ![NOT DONE](images/red.png)

    * [5.2.7 Artifact Management](5/5.2.md#527-artifact-management) ![NOT DONE](images/red.png)

    * [5.2.8 User Management](5/5.2.md#528-user-management) ![NOT DONE](images/red.png)

        * [5.2.8.1 Authentication Management](5/5.2.md#5281-authentication-management) ![NOT DONE](images/red.png)

        * [5.2.8.2 Enable, disable & delete users](5/5.2.md#5282-enable-disable--delete-users) ![NOT DONE](images/red.png)

        * [5.2.8.3 User Role Management](5/5.2.md#5283-user-role-management) ![NOT DONE](images/red.png)

    * [5.2.9 Agent Management](5/5.2.md#529-agent-management) ![NOT DONE](images/red.png)

    * [5.2.10 UI Architecture](5/5.2.md#5210-user-interface-architecture) ![PENDING REVIEW](images/blue.png)

        * [5.2.10.1 Markup : HTML](5/5.2.md#52101-markup--html) ![PENDING REVIEW](images/blue.png)
        
        * [5.2.10.2 Styling: CSS, SASS](5/5.2.md#52102-styling--css-sass) ![PENDING REVIEW](images/blue.png)
        
        * [5.2.10.3 Scripting : JavaScript, jQuery and Prototype](5/5.2.md#52103-scripting-javascript-jquery-and-prototype) ![PENDING REVIEW](images/blue.png)

    * [5.2.11 APIs, CCTray & Feeds](5/5.2.md#5211-apis-cctray--feeds) ![NOT DONE](images/red.png)

* [5.3 Go Agent](5/5.3.md) ![DONE](images/green.png)
    
    * [5.3.1 Overview](5/5.3.md#agent-overview) ![DOME](images/green.png)

    * [5.3.2 Bootstrapper](5/5.3.md#agent-bootstrapper) ![DONE](images/green.png)

    * [5.3.3 Launcher](5/5.3.md#agent-launcher) ![DONE](images/green.png)

    * [5.3.4 Agent](5/5.3.md#agent) ![DONE](images/green.png)

* [5.4 Common](5/5.4.md) ![IN PROGRESS](images/yellow.png)

    * [5.4.1 Plugin Architecture](5/5.4.1.md) ![IN PROGRESS](images/yellow.png)

    * 5.4.2 Agent - Server Communication ![NOT DONE](images/red.png)

* [5.5 Build Infrastructure](5/5.5.md) ![DONE](images/green.png)

    * [5.5.1 Build, Test, Package](5/5.5.md#packaging) ![DONE](images/green.png)
    
         * [5.5.1.1 Maven modules](5/5.5.md#modules) ![DONE](images/green.png)
         
         * [5.5.1.2 Documentation Creation](5/5.5.md#documentation-creation) ![DONE](images/green.png)
         
         * [5.5.1.3  Pom conventions](5/5.5.md#pom-conventions) ![DONE](images/green.png)
         
         * [5.5.1.4 Jar Packaging](5/5.5.md#jar-packaging) ![DONE](images/green.png)
         
         * [5.5.1.5 TLB integration](5/5.5.md#tlb-integration) ![DONE](images/green.png)

    * [5.5.2 Installer Creation](5/5.5.md#installer-creation) ![DONE](images/green.png)

        * [5.5.2.1 Zip](5/5.5.md#zip) ![DONE](images/green.png)

        * [5.5.2.2 RPM](5/5.5.md#rpm) ![DONE](images/green.png)

        * [5.5.2.3 Debian](5/5.5.md#debian) ![DONE](images/green.png)

        * [5.5.2.4 Windows](5/5.5.md#windows) ![DONE](images/green.png)

        * [5.5.2.5 Mac OS X](5/5.5.md#mac-osx) ![DONE](images/green.png)

        * [5.5.2.6 Solaris](5/5.5.md#solaris) ![DONE](images/green.png)

#### 6. Features

* 6.1 [Dashboard](6/6.1.md) ![DONE](images/green.png)

    * [6.1.1 Personalise](6/6.1.md#611-personalise) ![DONE](images/green.png)

    * [6.1.2 Search](6/6.1.md#612-search) ![DONE](images/green.png)
    
    * [6.1.3 Pipeline Group(s)](6/6.1.md#613-pipeline-groups) ![DONE](images/green.png)
    
    * [6.1.4 Pipeline(s) and Ordering of pipeline instances](6/6.1.md#614-pipelines-and-ordering-of-pipeline-instances) ![DONE](images/green.png)
    
    * [6.1.5 Active Pipelines](6/6.1.md#615-active-pipelines) ![DONE](images/green.png)

* [6.2 Fan-in](6/6.2.md) ![DONE](images/green.png)

    * [6.2.1 Overview](6/6.2.md#overview) ![DONE](images/green.png)

    * [6.2.2 Pipeline Timeline](6/6.2.md#pipeline-timeline) ![DONE](images/green.png)

    * [6.2.3 Algorithm](6/6.2.md#algorithm) ![DONE](images/green.png)

    * [6.2.4 Corner Cases](6/6.2.md#corner-cases) ![DONE](images/green.png)

    * [6.2.5 Extensions](6/6.2.md#extensions) ![DONE](images/green.png)

* [6.3 Value Stream Map](6/6.3.md) ![PENDING REVIEW](images/blue.png)

    * [6.3.1 Overview](6/6.3.md#overview) ![PENDING REVIEW](images/blue.png)

    * [6.3.2 Layer Assignment](6/6.3.md#layer-assignment) ![PENDING REVIEW](images/blue.png)

    * [6.3.3 Dummy Node Creation](6/6.3.md#dummy-node-creation) ![PENDING REVIEW](images/blue.png)

    * [6.3.4 Edge Cross Minimisation](6/6.3.md#edge-cross-minimization) ![PENDING REVIEW](images/blue.png)

    * [6.3.5 Corner Cases](6/6.3.md#corner-cases) ![PENDING REVIEW](images/blue.png)

    * [6.3.6 Extensions](6/6.3.md#extensions) ![PENDING REVIEW](images/blue.png)

* [6.4 Compare Pipeline](6/6.4.md) ![PENDING REVIEW](images/blue.png)

    * [6.4.1 Overview](6/6.4.md#641-overview) ![PENDING REVIEW](images/blue.png)
    
    * [6.4.2 Implementation](6/6.4.md#642-implementation) ![PENDING REVIEW](images/blue.png)
    
    * [6.4.3 Corner cases](6/6.4.md#643-corner-cases) ![PENDING REVIEW](images/blue.png)

* [6.5 PackageRepository](6/6.5.md) ![PENDING REVIEW](images/blue.png)

    * [6.5.1 Overview](6/6.5.md) ![PENDING REVIEW](images/blue.png)

    * [6.5.2 Capturing Configuration](6/6.5.md#package-configuration) ![PENDING REVIEW](images/blue.png)

    * [6.5.3 Retrieving Package Revisions](6/6.5.md#package-revision) ![PENDING REVIEW](images/blue.png)

* 6.6 Command Repository ![NOT DONE](images/red.png)

* [6.7 Environments](6/6.7.md) ![PENDING REVIEW](images/blue.png)

* 6.8 Templates ![NOT DONE](images/red.png)

* 6.9 Shine ![NOT DONE](images/red.png)

    * 6.9.1 Test Artifact Parser ![NOT DONE](images/red.png)

    * 6.9.2 Reporting ![NOT DONE](images/red.png)

    * 6.9.3 Stage Graph ![NOT DONE](images/red.png)

* [6.10 OAuth Gadgets](6/6.10.md) ![PENDING REVIEW](images/blue.png)

* [6.11 Backup](6/6.11.md) ![PENDING REVIEW](images/blue.png)

#### 7. CD in practice

* 7.1 Build Go Using Go ![NOT DONE](images/red.png)

* [7.2 Test Infrastructure](7/7.2.md) ![PENDING REVIEW](images/blue.png)

    * [7.2.1 Rails specs using RSpec](7/7.2.md#721-rails-specs-using-rspec) ![PENDING REVIEW](images/blue.png)

    * [7.2.2 Java testing using JUnit](7/7.2.md#722-java-testing-using-junit) ![PENDING REVIEW](images/blue.png)

    * [7.2.3 Javascript testing using JsUnit Tests](7/7.2.md#723-javascript-testing-using-jsunit-tests) ![PENDING REVIEW](images/blue.png)

    * [7.2.4 Acceptance & Regression tests using Twist](7/7.2.md#724-acceptance--regression-tests-using-twist) ![PENDING REVIEW](images/blue.png)
    
    * [7.2.5 Performance Tests](7/7.2.md#725-performance-tests) ![PENDING REVIEW](images/blue.png)
    
    * [7.2.6 Test Parallelization](7/7.2.md#726-test-parallelization) ![PENDING REVIEW](images/blue.png)

* 7.3 Continuous Deployment ![NOT DONE](images/red.png)

#### 8. Miscellaneous

* 8.1 [Technical Debt](8/8.1.md) ![DONE](images/green.png)
