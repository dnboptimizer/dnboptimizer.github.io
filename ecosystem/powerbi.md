# Power BI

To setup a Power BI reports follow the instructions below.  
For more information see [Power BI](https://powerbi.microsoft.com/en-us/).

**Note: Power BI/Common Data Service integration is only support in the US.**

## Activate Power BI
Request activation of Power BI in your tenant: [aka.ms/cdspowerbi](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRwWp5miMBjRAhmGSAULZVM5URVBXNE01M1NSUVFDWlpQVUhNNzQ0MUdINi4u)

**Note: This may take several hours or into the next business day.**

## Enable Database
1. From the PowerApps [website](https://web.powerapps.com) click on settings and select the "Admin center" menu item.
2. Select the Environment tab.
3. Select the environment you want to enable Power BI reporting in.
4. Select the Database tab.

**Note: If your database is active you will see "Your database is currently visible to Power BI users." If your database is not active click the Active button.**

## Create Perspectives
1. From the PowerApps [website](https://web.powerapps.com) click on Common Data Service.
2. Select Perspectives.
3. Select New perspective and fill in the details for Business Profile.

## Power BI Desktop
1. Download the Power UI Desktop application [here](https://powerbi.microsoft.com/en-us/desktop/).
2. Download the <a href="/assets/dnb_Optimizer_1_0_0_0_powerbi.pbit" download>D&B Template</a>. 
3. Launch the Power UI Desktop application, import the D&B template and sign in.
4. Select Home > Edit Queries > Data source settings, select your CDS environment and from the list select the BusinessProfile perspective.
5. The report should now populate with the data from your CDS Business Profile entity.

## Publish Report
1. Select Home > Publish and sign in.
2. Select a destination to publish the report too.

## Power BI Web
1. Sign in to [Power BI](https://powerbi.microsoft.com).
2. Select the workspace you published the report too, select the Reports tab and select the report.
3. Click the pin icon on the top right corner to Pin to dashboard, select a dashboard and click Pin.

**Note: You must put the report in a dashboard to embed it into a dynamics 365 dashboard.**
 
## Dynamics 365 Reports
1. Sign in to Dynamics 365.
2. Select Settings > Administration > System Settings, select the Reporting tab.
3. Set the Allow Power BI visualization embedding to Yes and click OK.
4. Select Sales > Dashboards.
5. Select NEW > Power BI Dashboard.
6. Your Power BI Dashboard should be available in the Dashboard drop down, select it and click Save.