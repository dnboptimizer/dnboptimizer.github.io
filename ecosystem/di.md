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