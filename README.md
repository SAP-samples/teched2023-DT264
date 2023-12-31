[![REUSE status](https://api.reuse.software/badge/github.com/sap-samples/teched2023-DT264)](https://api.reuse.software/info/github.com/sap-samples/teched2023-DT264)

# DT264 - Use ABAP Cloud to build extensions for SAP S/4HANA Cloud, Public Edition

## Description

This repository contains the material for the SAP TechEd 2023 session called _DT264 - Use ABAP Cloud to build extensions for SAP S/4HANA Cloud, Public Edition_.  

Developer extensibility as defined by SAP basically encompasses two activities 

1. Develop custom code to implement your own business logic. Here you can make use of existing API's from SAP that have been released for that purpose.
2. Extend an existing RAP Business Object delivered by SAP so that additional business functionality is added. Such an extensible RAP business object will usually reside in another software components or it is an existing SAP delivered RAP BO that is extensible. Both can be optimized and their functionality can be adapted to your specific business requirements.

## Overview

This session introduces attendees to the ABAP Cloud programming model and how this can be leveraged to build own code in SAP S/4HANA Cloud ABAP Environment
or how you can extend an existing RAP Business Object using the ABAP Cloud programming model.   

## Requirements

The requirements to follow the exercises in this repository are:

- You have installed the latest version of the ADT tools    
- You have a user and demo system access

as described in our [Getting Started](exercises/ex0/) section.   


## Exercises

In the _Getting Started_ section we describe how you get a user in the SAP S/4HANA Cloud ABAP Environment which you will have to use to perform the exercises in this session. You will create an ABAP Cloud project to connect the demo system. Here you will generate an extensible managed Business Object (BO) with one entity _Shop_ with generic transactional behavior - i.e. CRUD: Create, Read, Update, and Delete. For your convenience, the class **`ZDMO_GEN_RAP630_SINGLE`** is provided to you to generate the package  **`ZRAP630_###`** alongside with the aforementioned RAP business object after execution.

In _Exercise 1_ you will learn how to leverage the released RAP BO `I_BankTP` . 

In _Exercise 2_ you will _extend the behavior_ of the base RAP business object that has been generated at the end of the Getting Started section. You will learn how to extend the behavior of the base RAP BO by validations, determinations and side effects. 

In _Exercise 3_ you will then continue to _extend the data model_ with additional fields. This requires you to perform several steps and you have to create quite a lot of repository objects. (There is a plan to provide a Generator for that.)  

In _Exercise 4_ you will continue to _extend the behavior_ of the base RAP business object by adding an action. Since actions can only added via an extension to fields that have been added via an extension as well, adding an action via an extension must be performed after Exercise 3.   


So let us start and have a look at the _Getting Started_ section.

- [Getting Started](exercises/ex0/)
- [Exercise 1 - Consume a released RAP BO](exercises/ex1/)
- [Exercise 2 - Extend the behavior (determinations, validations, side-effects)](exercises/ex2/)
- [Exercise 3 - Extend the data model (add additional fields)](exercises/ex3/)
- [Exercise 4 - Extend the behavior (add an action)](exercises/ex4/)


## Online Help

https://help.sap.com/docs/abap-cloud/abap-rap/develop-rap-extensions
https://help.sap.com/docs/SAP_S4HANA_CLOUD/6aa39f1ac05441e5a23f484f31e477e7/1b345c53060846b091f55ea901e21ae7.html

## Contributing
Please read the [CONTRIBUTING.md](./CONTRIBUTING.md) to understand the contribution guidelines.

## Code of Conduct
Please read the [SAP Open Source Code of Conduct](https://github.com/SAP-samples/.github/blob/main/CODE_OF_CONDUCT.md).

## How to obtain support

Support for the content in this repository is available during the actual time of the online session for which this content has been designed. Otherwise, you may request support via the [Issues](../../issues) tab.

## License
Copyright (c) 2023 SAP SE or an SAP affiliate company. All rights reserved. This project is licensed under the Apache Software License, version 2.0 except as noted otherwise in the [LICENSE](LICENSES/Apache-2.0.txt) file.
