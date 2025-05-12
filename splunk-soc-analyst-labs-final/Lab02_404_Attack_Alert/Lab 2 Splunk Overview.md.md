# Lab 2: 404 Attack Alert

## Description
This lab demonstrates how to perform a Splunk detection or engineering task. It simulates a real SOC task using Splunk Enterprise or Splunk Cloud.

## Key Skills Practiced
- ✅ Writing custom SPL queries
- ✅ Building dashboards or alerts
- ✅ Using lookups or workflow actions
- ✅ Practicing detection engineering concepts

## SPL Example
```spl
index=apache_day1 status=404
| stats count by uri_path
| where count > 10
```

## Try It Yourself

① Upload sample logs (if applicable) using "Add Data" in Splunk.  
② Open the Search & Reporting app.  
③ Paste the SPL query and run it.  
④ Save the search as a report, alert, or dashboard panel.  
⑤ Visualize, enrich, or correlate events as needed.

## Screenshots
Visual output here:

![Lab 2 Screenshot](Lab2.png)

## Notes
This lab is designed to be modular. You can enhance it with additional SPL, saved searches, or dashboard panels as your skills grow.
