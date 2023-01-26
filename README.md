# AWS Static Website S3
Launching a static website adaobionyeakagbu.com on AWS S3 bucket and CloudFront.

![static website](https://user-images.githubusercontent.com/66325142/213918006-b229e564-3271-4fb7-979a-aa702c6c0fac.png)

Goals of this project include:
- Create a simple html website
- Register a New Domain Name in Route 53
- Create an S3 Bucket and enable static website hosting
- Create a Record Set in Route 53 and link to bucket
- Host website on S3 bucket
- Request a certificate from AWS Certificate Manager
- Set up CloudFront for caching of the site

## Phase 1: Create S3 Bucket
First, i created a bucket using the name of the website name I will register on DNS i.e (adaobionyeakagbu.com). I left all the default settings except the 'Block Public Access settings for this bucket' which I disabled to allow public access to this bucket. 

![2](https://user-images.githubusercontent.com/66325142/214683820-1804f324-84e9-4555-8efd-d18d3fb7e3aa.png)

After that, I edited static website hosting settings on the properties of the bucket and enabled it. The hosting type needs to be 'Host a static website' since this is the main bucket.
![3](https://user-images.githubusercontent.com/66325142/214688621-c870aec7-7d70-4d97-a4e4-005c14e61763.png)

Next, the permissions of the bucket needs to be set with a bucket policy. The policy used is in the repo. It sets a get request for the objects in the bucket, and the bucket name needs to be defined.
![4](https://user-images.githubusercontent.com/66325142/214698545-2bdbf39f-6346-45aa-ab3c-8a96041cf8c6.png)
That's all for the bucket for now.

## Phase 2: Register Domain Name via Route 53

## Phase 3: Register for an SSL certificate from AWS Certificate Manager for Secure access

## Phase 4: Set up CloudFront for caching

## Phase 5: Build fault-tolerant and secure three-tier Network VPC architecture from scratch


