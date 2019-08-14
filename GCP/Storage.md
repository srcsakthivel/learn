## Getting Strated

Login from Cloud Shell 
 ``` 
 gcloud auth login
 ```
 
## Storage
 - For unstructured data
 - object store
 
 
## Types
 - Cold Data
  - Cold Line - Once a year
 - Cool Data
  - NearLine - Once a month
 - Hot Data
  - Regional - For specific region
  - Multi Regional - For anywhere in trhe world
 


## gsutil Commands

- Create a bucket 
  ```
  gsutil mb gs://<BucketName>/
  ```
  
- Create a reginal bucket
  ```
  gsutil mb -c regional -l us-east1  gs://myfb-personnel-regional-bucket/
  ```
  
- List Bucket
  ```
  gsutil ls
  ```

- Bucket detail
  ```
  gsutil ls -L -b gs://myfb-personnel-bucket/
  ```
 
- Upload file
  ```
  gsutil cp employee_names.txt gs://myfb-personnel-bucket/documents/
   ```
- List Files
  ```
  gsutil ls gs://myfb-personnel-bucket/documents/
  ```
  
- List Recruse
  ```
  gsutil ls gs://myfb-personnel-bucket/**
  ```
  
- Rename a FIle
  ```
  gsutil mv -p gs://myfp-employee-storage-bucket/documents/employee_names.txt gs://myfp-employee-storage-bucket/documents/employees_name.txt
  ```
  
- Copy 
  ```
  gsutil cp -p gs://myfp-employee-storage-bucket/documents/employees_name.txt gs://"myfp-nearshore-storage-bucket/documents/employees_name.txt"
  ```

