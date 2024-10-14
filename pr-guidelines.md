
## What?
I've added support for LB log service access to S3 bucket. It includes SSE encryption and allow lb service to write logs. For more background, see ticket 
#ADO-123.
## Why?
Default standard is CMK, however LB access logs doesn't support CMK and hence SSE encryption is only viable path for successful log ingestion in to bucket
## How?
Update Bucket with SSE encryption and allow lb service.
## Testing?
I've added coverage for testing all new methods. I used Faker for a few random user emails and names.
## Screenshots (optional)
0
## Anything Else?
<details>
  <summary>Terraform Plan</summary>
  
  ## After running plan: 
</details> 