# **gost-s3uploader**

1. Creates folders in C://data to transfer files.
2. Creates an AWS config file in C://Users/%USERPROFILE%/.aws. ***(See example config file below)***
3. Logs into AWS GOST Prod Env with 'analyst' profile.
4. Transfers file to S3://gost-internal-upload.

# **Requirements**
AWS CLI v2
Access to AWS GOST Prod Env

## **Login**
1. Enter "analyst" when prompted to login.
2. Your defualt browser will pop-up asking you to log in or confirm authorization.

## **Example config file**
[profile analyst]<br>
**sso_start_url**= https://start.us-gov-home.awsapps.com/directory/gost-smx-com<br>
**sso_region** = us-gov-west-1<br> 
**sso_account_id** = 501979927634_SSO-GOSTAnalyst<br>
**sso_role_name** = SSO-GOSTAnalyst<br>
**region** = us-gov-west-1<br>
**output** = json<br>

If you want to check your upload, click on the link below. You will only be able to access the 'gost-internal-upload' bucket and read objects in the bucket.<br>

**s3://gost-internal-upload**: https://console.amazonaws-us-gov.com/s3/buckets/gost-internal-upload?region=us-gov-west-1<br>







