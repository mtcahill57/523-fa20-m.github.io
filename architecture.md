---
title: Application Architecture
---
### [Home](https://mtcahill57.github.io/523-fa20-m.github.io/) \| [Project](project.md) \| [Team](team.md) \| [Deliverables](deliverables.md) \| [Schedule & Journal](journal-sched.md)

___

1. App Platform
* Summary
  * In order to deploy an app efficiently over a wide range of devices, we decided to develop an Android app.
* Problem
  * We need the app to run responsively and be accessible on a wide array of devices. This is a problem because the survey conditions will encourage minimizing time-to-complete as the main factor in usability.
* Constraints
  * We want the app to be very responsive, and potentially able to store results locally for a time if a connection to the database cannot be established. 
* Options
  * Android App
    * Pros: 
      * Available on many devices
      * Relatively easy to make
      * Ryan has experience with frontend for Android
      * Can be used without internet
    * Cons: 
      * Might be less popular than iOS app
      * May have to change implementation with Android updates
  * iOS App
    * Pros: 
      * iPhone popularity increases availability of app
      * Can be used without internet
    * Cons: 
      * Learning swift would add difficulty to project
  * Web App
    * Pros: 
      * Can be accessed from any device, including computers
    * Cons: 
      * Slower and less responsive
      * Server access can be cut off
      * Can’t be used without internet
  * Progressive Web App
    * Pros: 
      * Can be accessed by more devices
      * More responsive than regular web app
    * Cons: 
      * Harder to deploy changes
      * Not as reliable as native app
      * Installation may be confusing for users
* Rationale
  * We chose to do an Android app for this project because it aligned the most with our current knowledge and fit our use-case well. Our client offered from the beginning to have us work on the project after the semester, meaning an iOS app can be completed in the future to round out the native app device space.
2. Data Type
* Summary
    * In order to create and manage our data easily, we decided to format our survey information in JSON.
* Problem
    * We want the data to be easily written and parsed to allow for simple integration with our database.
* Constraints
    * Whatever data type we choose must be easily transmittable and able to be inserted in our database, either directly or by a simple parsing process.
* Options
  * JSON
    * Pros:
      * Creation is simple fill in the blank
      * Interfaces directly with most database systems
    * Cons: 
      * Transition to or integrating with CSV may be difficult
  * HTTP raw text
    * Pros: 
      * Data can be input as simple string in whatever format we want
    * Cons: 
      * Data has to be parsed into another format to deliver it to database
* Rationale
  * We chose to write our data to JSON format because it can be directly inserted into most databases, and the creation and parsing is simple.
3. Database
* Summary
  * In order to store our data in a simple and accessible but scalable manner, we chose to use Amazon DocumentDB as our database.
* Problem
  * We need a database which can efficiently and securely store the information collected in the app in a format which is easy to access and analyze.
* Constraints
  * We need a database that can export to csv as per the client's request.
* Options
  * SQL
    * Pros:
      * Flexibility
      * Good with queries
    * Cons:
      * Server setup more involved
      * Harder to scale automatically
  * Amazon DocumentDB
    * Pros: 
      * Persistent storage
      * Easy to set up
      * Scalable
      * Interface with MongoDB, which has API's
      * Secure, supports storing multiple copies of data to prevent losses
    * Cons: 
      * Limited interface options
* Rationale
  * We chose to work with Amazon DocumentDB because the service is simple and reliable. The processes of importing and exporting of data are well documented and allign with the rest of our project structure.
___
[Assignment Page](https://comp523.cs.unc.edu/application-architecture/)
