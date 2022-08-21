

[Project Home Webpage](https://asadidebuger.github.io/wpcrudrest-docs/)
# WPCrudRest
### A Powerful Wordpress CRUD & RESTful plugin Generator *(Eclipse plugin)*
## Introduction
This artifact is the result of a master's thesis in Isfahan University and contains set of Eclipse plugins that enable you to generate a WordPress plugin by graphical modelling. We use Model-Driven approach to generate codes from model.     
WPCrudRest is currently only available as a plugin for Eclipse. It used [Sirius](https://www.eclipse.org/sirius/) to provide a graphical modelling environment and use [Acceleo](https://www.eclipse.org/acceleo/download.html) to transform models to code.
## Please participate in the evaluation
You can participate in the evaluation of the WPCrudRest framework through the following links:
* **[Evaluation participate (English language)](https://github.com/asadidebuger/wpcrudrest-docs/blob/main/_posts/2022-08-20-evaluation-en.markdown)**

&#x202b;
* **[مشارکت در ارزیابی (فارسی)](https://github.com/asadidebuger/wpcrudrest-docs/blob/main/_posts/2022-08-20-evaluation-fa.markdown)**
## Installation 
### *Tested on [Eclipse Modeling Tools 2022-06](https://www.eclipse.org/downloads/packages/release/2022-06/r/eclipse-modeling-tools)  & [windows 10 64X OS](https://www.microsoft.com/en-us/software-download/windows10)  with  [Java 11](https://www.oracle.com/java/technologies/javase/jdk11-archive-downloads.html)*

### You can follow the steps below to deploy and use the framework:

_Note: You can follow [**this link**](https://www.cloudways.com/blog/install-wordpress-locally/) to **deploy WordPress on your personal computer** if you are unfamiliar with WordPress!_

### A. Install Eclipse
1. Download [Eclipse Modeling Tools ](https://www.eclipse.org/downloads/packages/release/2022-06/r/eclipse-modeling-tools)
2. Install (unzip) downloaded Eclipse package

### B. Configure Eclipse and Install required plugins

1. Download latest [WPCrudRest package](https://github.com/asadidebuger/WPCrudRest/releases/latest)
2. Unzip downloaded package and copy [dropins](https://github.com/asadidebuger/WPCrudRest/tree/main/dropins "dropins") directory to eclipse installation path (e.g  C:\Program Files\eclipse)
3. Execute Eclipse
4. Install [Acceleo](https://www.eclipse.org/acceleo/download.html) plugin
5. Install [Sirius](https://www.eclipse.org/sirius/)  plugin *(preinstall in newer versions)*
6. Restart Eclipse

### C. Create new Modeling Project
1. Click on "File" menu item
2. Choose "New" ->" Other" item from "File" menu
3. In "Select a wizard" window, search for "Sirius" group and expand it by click
4. Choose "Modeling Project" and click "Next"
5. Select a name for project and type it in "Project name" field
6. Click on "Finish" button to create modeling project

### D. Create "Crudrest Model"
Note: Field type repository model use to define entities field types and if not exist modelling and generating code is not possible! this is recommended to use [exist pre-built field repository model](https://github.com/asadidebuger/WPCrudRest/blob/main/models/FieldTypeRepo.crudrest)!
1. Copy [FieldTypeRepo.crudrest](https://github.com/asadidebuger/WPCrudRest/blob/main/models/FieldTypeRepo.crudrest "FieldTypeRepo.crudrest") from [models](https://github.com/asadidebuger/WPCrudRest/tree/main/models "models") directory to project model *(or root)* directory
2. You can simply copy one of sample models from [models](https://github.com/asadidebuger/WPCrudRest/tree/main/models) repository directory)  and jump to next step
2. Right click on project root in Eclipse Project (or Model) explorer
3. Choose "New" ->" Other" item from popup menu
4. In "Select a wizard" window,  search for "Crudrest Model" an choose it
5. Click next and choose directory and a name *(with .crudrest extension)* to create model file and click "Next" button
6. Choose "Plugin Creator" from "Model Object" drop-down list
7. Click Finish to create model file

### E. Open WordPress Crudrest Plugin Model in graphical editor
1. Double click on representations.aird file
2. Enable CrudRestWPP from Presentation part
3. Double click on CrudRestWPP to open Sirius visual model editor
4. Edit model
5. Save it!

### F. Generate WordPress Plugin Code

1. If you want to deploy the plugin directly on your local WordPress, set "WP_HOME" path as Wordpress root directory in system environment 
   
        Windows OS:
                    setx WP_HOME WORDPRESS_PATH /M
        Example: 
                    setx WP_HOME C:\xampp7.1\htdocs\projects\crudrest /M
    [*Click here for more help*](https://dev.to/kapilgorve/set-environment-variable-in-windows-and-wsl-linux-in-terminal-3mg4)
   

2. Right click on model
3. Choose "WP Crud-Rest" -> "Generate WordPress Plugin" from popup menu
4. Plugin code will be generated in "generated WPP" directory on project root directory

## Guidance Videos
1. Download Eclipse modeling tools -> [Watch video](https://youtu.be/RB18NMginCs)
2. Install (extract) Eclipse modeling tools package -> [Watch video](https://youtu.be/AvLZi5cKzPc)
3. Download WPCrudRest -> [Watch video](https://youtu.be/MIR8y91KHbU)
4. Install Acceleo as Eclipse plugin -> [Watch video](https://youtu.be/qH5_xmrrvH0)
5. Deploy (install) WPCrudRest as Eclipse plugin -> [Watch video](https://youtu.be/mfCE0lGbDAE)
6. Create new modeling project -> [Watch video](https://youtu.be/WUnkY3NEJus)
7. Start modeling using graphical editor -> [Watch video](https://youtu.be/pJbHDgvNWM0)
## Screenshots
#### Graphical modeling editor screenshot:
![Graphical modeling editor screenshot](screenshots/graphical-modeling-screenshot.png)

#### Generate WordPress plugin code from model screenshot:
![Generate WordPress plugin code from model screenshot](screenshots/generate-code-screenshot.png)

#### Generated WordPress plugin code screenshot *(zip this directory and install it on Wordpress as plugin or just copy it to WordPress plugin directory)*:
![Generated WordPress plugin code screenshot](screenshots/generated-plugin-code-screenshot.png)
![Generated WordPress plugin code screenshot](screenshots/generated-plugin-code-screenshot2.png)![Generated WordPress plugin code screenshot](screenshots/generated-plugin-code-screenshot3.png)
___

#### WordPress plugin pages:
![WordPress plugin pages](screenshots/microhrm-pages.png)

#### WordPress plugin access controll (AC) page:
![WordPress plugin access controll (AC) page](screenshots/microhrm-options.png)

#### WordPress plugin list item page:
![WordPress plugin list item page](screenshots/microhrm-list-items.png)

#### WordPress plugin create (or edit) item page:
![WordPress plugin create (or edit) item page](screenshots/microhrm-edit-item.png)

#### WordPress plugin RESTful webservice tested by RESTClient:
![WordPress plugin RESTful webservice tested by RESTClient](screenshots/microhrm-rest.png)
![WordPress plugin RESTful webservice tested by RESTClient](screenshots/microhrm-rest2.png)
