# Airflow: Loading data from S3 to Redshift

This code vignette teaches you how to load data from S3 to redshift **the hard way**

PS: it's easy, but there's an easier method, i.e, using the **S3ToRedshiftOperator**

This example stages some data on songs in Redshift and loads said data into **Songs** and **Artists** tables. Quality checks and data partitioning is not applied to the input data.

## Loading the data

The original data can be retrived from **s3://udacity-dend/song_data**

Check the **stage_songs** in **sql.py** for the copy command that loads the data from S3 to Redshift

The airflow dag is defined in **S3-to-Redshift.py**