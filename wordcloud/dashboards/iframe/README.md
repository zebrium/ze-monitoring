# WORD CLOUD DASHBOARD FOR IFRAMES

Zebrium **Machine Learning for Logs** provides an aggregated Word Cloud that can be embedded into any monitoring dashboard that supports iFrames (e.g. Datadog).

## In Zebrium

### Select the Word Cloud Dashboard URL for use in the iFrame

1. From the **User** menu area, click on the **Settings Menu**.
2. Click the **Monitoring Dashboard** menu item.
3. Navigate to the **Other** tab
4. Copy the URL and save for use when Adding the Word Cloud Dashboard to your Monitoring Tool.

## In your Monitoring Tool (e.g. Datadog)

### Adding the Word Cloud Dashboard to your Monitoring Tool

1. Paste the URL from step 4 above into the iFrame in your monitoring tool that will contain the Zebrium Word Cloud.

**Notes**
* Use the **refresh** component of the URL to specify the frequency to refresh the Word Cloud. Default is **10** seconds.
* Use the **svc_grp** (service group) component of the URL to match any service group defined in Zebrium. Default is **All** service groups.
