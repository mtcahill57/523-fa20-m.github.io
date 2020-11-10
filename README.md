---
title: README
---

# Pet Obesity Survey App

![Logo](apop-logo.png)

## For The Association for Pet Obesity Prevention, under Dr. Ernie Ward & Prof. Jeff Terrell
### Comp 523 Fall 2020 - Group M: Matthew Cahill, Ryan Humphrey, Robbie Errico

**Overview**

Veterinarians currently record information on pet obesity on paper, which must then be manually translated to digital data before it can be analyzed, which is inefficient. We will attempt to create an app to streamline this process, while still being simple and intuitive for use.

**Getting started**
- Once deployed, the app should run on any Android device. 
- To work with the repository in Android Studio, you’ll need the Amplify CLI and an Amazon Web Services account.
- docs.amplify.aws/lib/project-setup/prereq/q/platform/android
- Follow the instructions for setup and 
- To run locally, just emulate a device on Android Studio and run the built project
- Warranty: when (in terms of date or commit) were these instructions last tested and verified to work, by whom, and on what operating system?

**Testing**
- Android Studio can run the test suite by changing the run configuration to “Run Tests” in Android Studio
- Unit tests in the test suite can be run through Android Studio, integration tests can be 
- Any other test-related commands to know about, e.g. a different command for unit tests vs. integration tests?

**Deployment**
- Where does the production system live? How would a new developer get access to it?
- The project will be linked to an AWS backend, which you must configure for yourself. We recommend creating a Lambda function to consolidate the S3 data into a DynamoDB database.
- Continuous Deployment is not yet enabled.

**Technologies used**
- List which technologies were chosen.
- Mention where in the repository the ADRs live. (Add them to the repository if they’re not already there.)

**Contributing**
- A new developer to the project should get access to the repository (a contributor role if applicable).
- Does a new developer need to get access to any systems (e.g. the GitHub repository, Trello) before he or she is able to contribute?
- Are there any style, testing, or process conventions that a new developer should know about?
- Project Site: mtcahill57.github.io/523-fa20-m.github.io

**Authors**
- Frontend development was led by Ryan Humphrey.
- Backend integration was researched and developed by Robbie Errico and Matthew Cahill.

**License**
- What license applies to the source code? I recommend a liberal open-source license like the MIT license or the BSD license, so that your client can have the legal right to use and extend your work later in whatever way they would like. (However, teams with an IP agreement with their client should be careful not to pick something without getting their client’s approval first.)

**Acknowledgements**
- We'd like to thank Jeff Terrell, Jim Fletcher, and <> for their guidance and supoort with this project
