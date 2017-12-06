# Data Integration

To setup a data integration project in PowerApps follow the instructions below.
For more information see [Microsoft's introduction to Data Integration](https://docs.microsoft.com/en-us/dynamics365/unified-operations/dev-itpro/data-entities/data-integration-cds). You then reference those connections in a Data Integration project.

Before you can work with a Data Integration project, you must provision a connection for each system that you intend to work with in the Microsoft PowerApps portal. You then reference those connections in a Data Integration project.

1. From the PowerApps [website](https://web.powerapps.com) click on settings and select the "Admin center" menu item. ![logo](assets/settings_cog.png "Settings")
2. Then select the Data integration tab.
3. Choose Connection sets.

**Note: Before you create a connection set you need to create a Connection to Dynamics 365. To do this go to Powerapps, select your environment from the environments drop-down, click the "Connections" tab on the left and click the "New connection" button on the top right. From the list of connections select the Dynamics 365 connection and click the "Create" button.**

## Connection Sets
Connection sets are a collection of two more connections, organization mapping information, and integration keys that can be reused among projects.

1. Click the "Add connection set" link or the "New connection set" button and fill in the details. 
  1. Give the Connection set a name.
  2. Select a Connection & Environment for Dynamics 365.
  3. Select a Connection & Environment for Common Data Service.
  4. Organizations:
    1. Enter your Organization for Dynamics 365 for Sales. (Which you can get from your Dynamics 365 domain).
    2. Enter your Organization for Common Data Service. (Which you can get from the Organization entity in CDS; select the Data tab and scroll to the ORGANIZATION ID column)
2. Click "Create".

**Note: While you are free to choose any name you like we suggest something like D365SalesAccstoCDSSalesAccs so you can see from the name which data the connection set represents.**

## Projects
Projects enable the flow of data between systems.

1. Click "New project" and fill in the details.
2. Give the project a name.
3. Select the "Accounts (Sale to CDS)" template and click next.
4. Select Connection sets and click next.
4. Select an Organization and click next.
5. Read the privacy notice and consent and click create.

## Run/Schedule Project
Now everything is setup we can run/schedule the project.

1. Go back to Projects.
2. Select a Project from the list.
3. Select the Scheduling tab.
  1. Leave as Run manually and click the Run project icon in the top right corner.
  2. Or select Recur every and pick your settings and click the "Save schedule".
  
**Note: You must run or schedule the project to run at least once before you create a template.**  
**Note: We recommend scheduling the project to recur every 5 minutes.**