# WORD CLOUD DASHBOARD FOR GRAFANA

Zebrium **Machine Learning for Logs** provides an aggregated Word Cloud that can be embedded into your Grafana dashboard.

## In Zebrium

### Select the Authorization Method for your Grafana Datasource

Zebrium provides two authorization methods when defining the Datasource in Grafana. Header-based authorization and URL-based authorization. Choose the appropriate one for your setup.

1. From the **User** menu area, click on the **Settings Menu**.
2. Click the **Monitoring Dashboard** menu item.
3. Navigate to the **Grafana** tab
4. If using **Header-Based Authorization**, copy the **Data Source URL** and **Header Value** and save for use when **Adding the Word Cloud Data Source to Grafana**.
5. If using **URL-Based Authorization**, copy the **Data Source URL** and save for use when **Adding the Word Cloud Data Source to Grafana**.

## In Grafana

### Prerequisites

The following must be configured in Grafana:

* CSV datasource (https://grafana.com/grafana/plugins/marcusolsson-csv-datasource/)
* DynamicText panel (https://grafana.com/grafana/plugins/marcusolsson-dynamictext-panel/)

### Adding the Word Cloud Data Source to Grafana

1. Create a new datasource from CSV. Name it Ze-CSV.
2. Copy the Data Source URL that was saved from step 4 or 5 above into the URL field.
3. If using Header-Based Authorization:
   * Under the section **Custom HTTP Headers** click **Add header**
   * In the **Header** field, add the string **Authorization**
   * In the **Value** field, paste **Header Value** from step 4 above.
4. Click **Save & test**

### Adding the Word Cloud Dashboard to Grafana

1. Download the Zebrium Word Cloud Dashboard JSON definition file from github:
  ```
   https://raw.githubusercontent.com/zebrium/ze-monitoring/master/wordcloud/dashboards/grafana/Ze-Word-Cloud.json
  ```
2. From the left-hand navigation panel, select **Dashboards/Manage**
3. Click on **Import**
4. Click on **Upload JSON file**
5. Select the file that was donwloaded in Step 1.
6. Select CSV data source Ze-CSV
7. Click **Import**
