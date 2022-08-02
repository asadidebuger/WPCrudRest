[Project Home Webpage](https://asadidebuger.github.io/WPCrudRest/)
# WPCrudRest
### A Powerful Wordpress CRUD & RESTful plugin Generator *(Eclipse plugin)*
## Introduction
This artifact is the result of a master's thesis in Isfahan University and contains set of Eclipse plugins that enable you to generate a WordPress plugin by graphical modelling. We use Model-Driven approach to generate codes from model. 
WPCrudRest is currently only available as a plugin for Eclipse. It used [Sirius](https://www.eclipse.org/sirius/) to provide a graphical modelling environment and use [Acceleo](https://www.eclipse.org/acceleo/download.html) to transform models to code.
## Installation 
### *Tested on [Eclipse Modeling Tools 2022-06](https://www.eclipse.org/downloads/packages/release/2022-06/r/eclipse-modeling-tools)  & [windows 10 64X OS](https://www.microsoft.com/en-us/software-download/windows10)  with  [Java 11](https://www.oracle.com/java/technologies/javase/jdk11-archive-downloads.html)*
### A. Install Eclipse
 1.  Download [Eclipse Modeling Tools ](https://www.eclipse.org/downloads/packages/release/2022-06/r/eclipse-modeling-tools)
 2. Install (unzip) downloaded Eclipse package 

### B. Configure Eclipse and Install required plugins

1. Download latest [WPCrudRest package](https://github.com/asadidebuger/WPCrudRest/releases/latest)
2. Unzip downloaded package and copy [dropins](https://github.com/asadidebuger/WPCrudRest/tree/main/dropins  "dropins") directory to eclipse installation path (e.g  C:\Program Files\eclipse)
3. Execute Eclipse
4. Install [Acceleo](https://www.eclipse.org/acceleo/download.html) plugin
5. Install [Sirius](https://www.eclipse.org/sirius/)  plugin *(preinstall in newer versions)*
6. Restart Eclipse

### C. Create new Modeling Project
1. Create new Modeling Project from Sirius section
2. Copy [FieldTypeRepo.crudrest](https://github.com/asadidebuger/WPCrudRest/blob/main/models/FieldTypeRepo.crudrest "FieldTypeRepo.crudrest") from [models](https://github.com/asadidebuger/WPCrudRest/tree/main/models "models") directory to project model *(or root)* directory
3. Double click on representations.aird file
4. Enable CrudRestWPP from Presentation part
5. Double click on CrudRestWPP to open Sirius visual model editor
6. Edit model
7. Save it!

### Generate WordPress Plugin Code

1. Right click on model
2. Choose 
will be completed...
