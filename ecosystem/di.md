# Data Integration

To setup a data integration project in PowerApps follow the instructions below.  
For more information see [Microsoft's introduction to Data Integration](https://docs.microsoft.com/en-us/dynamics365/unified-operations/dev-itpro/data-entities/data-integration-cds). You then reference those connections in a Data Integration project. 

Before you can work with a Data Integration project, you must provision a connection for each system that you intend to work with in the Microsoft PowerApps portal. You then reference those connections in a Data Integration project. 

1. From the PowerApps [website](https://web.powerapps.com) click on settings and select the "Admin center" menu item.
2. Then select the "Data integration" tab.

## Connection sets
Connection sets are a collection of two more connections, organization mapping information, and integration keys that can be reused among projects.
 
1. Click "New connection set" and fill in the details. 
  1. Give the Connection set a name.
  2. Select a Connection & Environment for Dynamics 365.
  3. Select a Connection & Environment for Common Data Service.
  4. Organizations:
    1. Enter the Organization for Dynamics 365 for Sales (e.g dnb).
    2. Enter the Organization for Common Data Service (e.g ORG001).
2. Click "Create".

## Projects
Projects enable the flow of data between systems.

1. Click "New project" and fill in the details.
2. Give the project a name.
3. Select the "Accounts (Sale to CDS)" template and click next.
4. Select a Connection set and click next.
4. Select an Organization and click next.
5. Read the privacy notice and consent and click create.

## Mappings
If your project does not have all of the attributes you wish to map, you can add a new mapping. We will add a mapping for the State/Province field.

1. Go back to Projects.
2. Select a Project from the list.
3. Select the Tasks tab and select your MAP.
4. Scroll down to address1_stateorprovince = MailingPostalAddress_PostalCode
5. Click on the equals sign.
6. On the Edit transform dialog click on Show JSON and copy the state/province mapping provided here.
7. Click Accept twice.

```JSON
[
  {
    "transformType": "ValueMap",
    "valueMap": {
      "Alabama": "AL",
      "Alaska": "AK",
      "Arizona": "AZ",
      "Arkansas": "AR",
      "California": "CA",
      "Colorado": "CO",
      "Connecticut": "CT",
      "Delaware": "DE",
      "Florida": "FL",
      "Georgia": "GA",
      "Hawaii": "HI",
      "Idaho": "ID",
      "Illinois": "IL",
      "Indiana": "IN",
      "Iowa": "IA",
      "Kansas": "KS",
      "Kentucky": "KY",
      "Louisiana": "LA",
      "Maine": "ME",
      "Maryland": "MD",
      "Massachusetts": "MA",
      "Michigan": "MI",
      "Minnesota": "MN",
      "Mississippi": "MS",
      "Missouri": "MO",
      "Montana": "MT",
      "Nebraska": "NE",
      "Nevada": "NV",
      "New Hampshire": "NH",
      "New Jersey": "NJ",
      "New Mexico": "NM",
      "New York": "NY",
      "North Carolina": "NC",
      "North Dakota": "ND",
      "Ohio": "OH",
      "Oklahoma": "OK",
      "Oregon": "OR",
      "Pennsylvania": "PA",
      "Rhode Island": "RI",
      "South Carolina": "SC",
      "South Dakota": "SD",
      "Tennessee": "TN",
      "Texas": "TX",
      "Utah": "UT",
      "Vermont": "VT",
      "Virginia": "VA",
      "Washington": "WA",
      "West Virginia": "WV",
      "Wisconsin": "WI",
      "Wyoming": "WY"
    }
  }
]
```

## Run/Schedule Project
Everything is setup. We can run or schedule the Project.

1. Go back to Projects.
2. Select a Project from the list.
3. Select the Scheduling tab.
  1. Leave as Run manually and click the Run project icon in the top right corner.
  2. Or select Recur every and pick your settings and click the "Save schedule".

## Known Issues
1. If your records in Dynamics 365 have an invalid Country/Region you will get an invalidEnums error on the mailingpostaladdress_country source field during the DI sync.