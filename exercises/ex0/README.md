# Getting started
In order to participate in this hands-on session, you MUST have installed the latest version of Eclipse and the latest version of the ABAP Development Tools (ADT) in Eclipse. Please check the following two short documents how to do this if you have not already done it:

[Install the ABAP Development Tools (ADT)](https://developers.sap.com/tutorials/abap-install-adt.html)

[Adapt the Web Browser settings in your ADT installation](https://github.com/SAP-samples/abap-platform-rap-workshops/blob/main/requirements_rap_workshops.md#4-adapt-the-web-browser-settings-in-your-adt-installation)

In addition to that, in this exercise you will:

1. Logon to the demo system
2. Create an ABAP Cloud Project
3. Start a helper class that will generate several artefacts needed for the remaining exercises.

## Logon to the demo system

Users and a demo system have been prepared upfront for you. You will receive the information in the session.


## Create an ABAP Cloud Project
Use the provided user and system information to create an ABAP Cloud Project like described here:
[Create an ABAP Cloud Project](https://github.com/SAP-samples/abap-platform-rap-workshops/blob/main/rap1xx/rap100/exercises/ex0/readme.md#create-an-abap-cloud-project-or-abap-project-in-adt)
(Please note that you need an ABAP Cloud project, the documentation covers both cloud and standard ABAP projects).

## Use class ZDMO_GEN_RAP630_SINGLE to generate your starter project

Now that you have created your ABAP Cloud project you will use class `ZDMO_GEN_RAP630_SINGLE` to generate packages which will be used in exercise 1 and an extensible RAP business object which will be used in the remaining exercises 2 and 3.

1. Right-click **Favorite Objects** and click **Add Object**.
   
2. Search for **`ZDMO_GEN_RAP630_SINGLE`**, select it and click **OK**.    

3. Right-click **`ZDMO_GEN_RAP630_SINGLE`**, select **Run As** > **ABAP Application (Console) F9**.

4. Now your packages `ZRAP630_###` and `ZRAP630_###_EXT` are created in some minutes and will contain everything you need. The suffix `###` denotes an arbitrary number (not necessarily connected to your user number), in the following exercises we call it your **group number**. Check the ABAP console for more information to get this number.

5. **⚠Copy the package names from ABAP console and the suffix for later use.**   
   In the "Project Explorer" right click on **Favorite Packages** and click on **Add Package...**.   
   Enter `ZRAP630_###` and and select **both** packages and click OK. 

## Summary

Now that you have onboarded to the SAP S/4HANA Cloud, Public Edition you can continue to - [Exercise 1](../ex1/README.md)
