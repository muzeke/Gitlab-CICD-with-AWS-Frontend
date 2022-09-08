# Simple Gitlab CICD Setup with AWS Frontend

## Validate your gitlab account if not yet validated

Unfortunately, you now need to validate your gitlab account to use gitlab runners. To do so, you'll need to connect a credit card with atleast 1 dollar. Gitlab won't charge you anything for this, they just need this to avoid spammers etc. (In the background, I noticed that they do charge 1$, but refund it again right away, hence the need to have atleast 1$)

## Gitlab

- Create .yml file
- Create CICD Setting variables
  - Frontend Bucket 
  - cloundfront invalidation

## AWS 
 
### IAM 
- create a user that you'll use to execute the deploy commands from gitlab 
- these user should have permissions to 
  - read / write on your S3 bucket (where your FEND files are deployed)
