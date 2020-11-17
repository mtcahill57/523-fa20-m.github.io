---
title: User Stories
---
### [Home](https://mtcahill57.github.io/523-fa20-m.github.io/) \| [Project](project.md) \| [Team](team.md) \| [Deliverables](deliverables.md) \| [Schedule & Journal](journal-sched.md)

___

# Pet Obesity Survey App
## Client Oriented Overview

- Major Project Pieces
  - Android App
    - User interface to collect survey and account data
    - Sends the collected information to an Amazon cloud
  - Amazon Web Services (AWS) Account
    - Holds two databases in the cloud
    - S3 for storage of account details
    - DynamoDB for storage of survey data
- Deployment
  - Our app will be deployed on the Android Google Play store for free, and will be able to connect to every cloud service without users setting anything up.
  - The AWS databases are linked to an account we have shared with the client.
- Management
  - The client can manage everything on the backend through the AWS Account.
    - The S3 buckets and DynamoDB tables can be deleted or locked to prevent unwanted costs if they wish to end the survey period and stop collecting data.
    - S3 object data and DynamoDB table data can be exported easily as individual json files or as csv of the entire data set.
- Costs
  - The DynamoDB and S3 autoscaling means that the account will be charged based on the number of input and output queries received. The number of surveys submitted, organizations registered, and unique user logins will determine this cost every month.
- Where does the code live? Is it open source or closed source? Does the client have a license to do what they want with it?
  - The code currently lives in a github repository. The code is open source and the client can do what they want with it. We may make changes to this based on meetings with the client as we progress after the semester.
- How to access the live app
  - The client will be able to access the live app through the Google Play store once it is deployed.
- “Need-to-have” user stories progress
  - All of our “need-to-have” features are complete except for one, which is partially complete. 
  - The partially complete feature is the ability for an admin web interface to manually create a clinic account. Right now this is possible through both the account creation screen, where anyone can register the org, or by uploading the relevant json file to the S3 bucket. The latter, however, will need the password to be manually hashed using our algorithm.
- “Nice-to-have” user stories progress
  - We have made some progress on the “nice-to-have” features. 
    - We are very close on finishing the implementation of camera use to take photos of pets.
    - We automatically link surveys to the organization and user that makes them.
    - We have a “Contact APOP” link in the survey thank you screen.
  - We’ve discussed other features with the client, and will work on them as needed.
- Highest priority next step
  - Our next priority is to manage the deployment of the app and finalize the pieces we have already in place.
