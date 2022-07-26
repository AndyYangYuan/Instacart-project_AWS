### ETL process using AWS DataBrew and AWS glue studio
The ETL process
![my picture](assets/images/ETL.png)
***
**1.Create datasets in AWS DataBrew**
AWS DataBrew can conviniently clean and normalise data for ananlytics tasks
![my picture](assets/images/dataset.png)
***
**2.Create projects and associative recipes**
![my picture](assets/images/projects.png)
- user_features_1
![my picture](assets/images/user1.png)
- user_features_2
![my picture](assets/images/user2.png)
- up_features
![my picture](assets/images/up.png)
- prd_features
![my picture](assets/images/prd.png)
***
**3.Create jobs to generate parquet files for each feature table and store them into AWS S3 Bucket**
![my picture](assets/images/jobs.png)
**4.Use glue studio to read the parquet files and join the four relational feature tables into one single table. Then export the dataframe as a single csv into s3 bucket**
![my picture](assets/images/csv%20file.png)