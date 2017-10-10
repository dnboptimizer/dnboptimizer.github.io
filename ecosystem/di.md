# Data Integration

To setup a data integration project in PowerApps follow the instructions below.

1. From the PowerApps [website](https://web.powerapps.com) click on settings and select the "Admin center" menu item.
2. Select the "Data integration" tab.

## Connection sets
1. Click "New connection set" and fill in the details. The connection will be from Dynamics 365 to CDS.
  1. Choose a connection: Dynamics 365 for Sales
  2. Environment: Choose one
  3. Choose a connection: Common Data Service
  4. Environment: Choose one
  5. Organizations:
    1. Dynamics 365 for Sales: Choose one (e.g dnb4)
    2. Common Data Service: Choose one (e.g ORG001)
2. Click "Create".

## Projects
1. Click "New project" and fill in the details.
2. Give the project a name and select the "Accounts (Sale to CDS)" template and click next.
3. Select a connection set and click next.
4. Select an organization and click next.
5. Read the privacy notice and consent and click create.

### Select project
1. Go back to projects.
2. Select a project from the list.
3. Select the scheduling tab.
  1. Set to recur every 5 minutes.
  2. Click "Save schedule".

## Mappings
1. Go back to projects.
2. Select a project from the list.
3. Select tasks tab and select your map.
4. Scroll down to address1_stateorprovince = MailingPostalAddress_PostalCode
5. Click on the equals sign.
6. On the Edit transform dialog click on Show JSON and add the state/province mapping

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

## Known Issues
1. If your records in Dynamics 365 have an invalid Country/Region you will get an invalidEnums error on the mailingpostaladdress_country source field during the DI sync.