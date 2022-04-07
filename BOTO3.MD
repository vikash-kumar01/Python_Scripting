### BOTO 3 MODULE

   #https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html
   
   
###  Using Client 
    
    import boto3
    client = boto3.client('s3')
    service = boto3.resource('s3')

### Client method to list buckets in AWS

    list_buckets= client.list_buckets()
           print(list_buckets)
### Print Buckets info based on some Key-value
    for bucket  in list_buckets["Buckets"]:
          print(bucket)

#### Print Bucket name Only
     for bucket  in list_buckets["Buckets"]:
           print(bucket["Name"])
           
           
### CREATE BUCKET 
  
    import boto3
    s3 = boto3.client('s3')
    bucket = s3.create_bucket(
    Bucket='myuniquebucket12324561',
    CreateBucketConfiguration={
        'LocationConstraint': 'us-east-2'
    }
    )
    print(bucket)
