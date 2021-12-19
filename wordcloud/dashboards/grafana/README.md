# WORD CLOUD DASHBOARD FOR GRAFANA

Zebrium **Machine Learning for Logs** provides an aggregated Word Cloud that can be embedded into your Grafana dashboard.

## In Zebrium

### Select the Authorization Method for your Grafana Datasource

Zebrium provides two authorization methods when defining the Datasource in Grafana. Header-based authorization and URL-based authorization. Choose the appropriate one for your setup.

1. From the **User** menu area, click on the **Settings Menu**.
2. Click the **Monitoring Dashboard Setup** menu item.
3. If using **Header-Based Authorization**, copy the **URL** and **Header** and save for use when **Configuring your Grafana Dashboard with Header-Based Authorization**.
4. If using **URL-Based Authorization**, copy the **URL** and save for use when **Configuring your Grafana Dashboard with URL-Based Authorization**.

## In Grafana

### Adding the Word Cloud Dashboard to Grafana using Header-Based Authorization

1. Create a new datasource from CSV. Name it Ze-CSV-HDR.
2. Add the URL that was saved from step 3 In Zebrium into the URL field.
3. Add a header using the format saved from step 3 In Zebrium.
4. Import the dashboard named **Ze-Cloud-HDR** from here:
   ```
   https://github.com/zebrium/ze-monitoring/blob/master/wordcloud/dashboards/grafana/Ze-Cloud-HDR.json
   ``` 

### Adding the Word Cloud Dashboard to Grafana using URL-Based Authorization

1. Create a new datasource from CSV. Name it Ze-CSV-URL.
2. Add the URL that was saved from step 4 In Zebrium into the URL field.
3. Import the dashboard named **Ze-Cloud-URL** from here:
   ```
   https://github.com/zebrium/ze-monitoring/blob/master/wordcloud/dashboards/grafana/Ze-Cloud-URL.json
   ```
