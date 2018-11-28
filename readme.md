# Introduction
For this task, I want you to create airflow dag(s) to import the sample files into google BigQuery.   
Data should be ingested into staging tables first before being moved to another dataset.   

Once created I want to walk through the code explaining what it does and explain any decisions or assumptions you have made.

# Details
- The files will be created daily and uploaded to gcp storage bucket so should be imported from there.   
- customer will always be a full extract and so only need to store most recent data.   
- sales will be incremental so need to keep history.   
- stock levels will be a snapshot at a given time.   