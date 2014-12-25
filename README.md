mobileCompany
=============

This project is example of multiple 'target' for one application. 

This is an android project which shows how to use resources for specific client. 

**Scenario**
There is an advertising company which have a basic app with a screen on which company's name , tagline and logo  are there. Suppose motorola and apple are clients of this advertising company. So now if company wants to manage single app and wants to export .apk using client specific resource. This project demonstrate best practice for such scenario.



**Steps**

 1. Created a new project named 'MobileCompany'
 2. Designed one sample activity layout with titleTextView, taglineTextView and Logo image
 3. Added two new library module named 'apple' and 'motorola'. [Stackover flow  question](http://stackoverflow.com/questions/16601299/how-to-create-a-library-project-in-android-studio-and-an-application-project-tha) shows how to add library
 4. Added company specific resources in associated library module. For this project resources are company's logo, tagline, app-name, company's theme color.
 5. Goto project structure -> app (from left bottom pane) -> dependancies
 6. Add new module dependency and choose appropriate module (either of motorola or apple)
 7. gradle will take time to configure it self. 
 8. Once gradle completes execution successfully run app.
 9. To change target got remove the older dependency which we included in step 6. and add other dependency.
 10. DONE!

**Outputs**
*Application for APPLE*
![Application for apple](https://lh5.googleusercontent.com/oZGCfsSpAO6ku9-aBF0JZn_u8YiNW-wQjCdiitSLwDEXJpUsY4OYyQmzfaKgVWQYaj-8iSQd3M8=w1511-h671)

*Application for MOTOROLA*
![Application for motorola](https://lh3.googleusercontent.com/LA17pMQgmYnxew9E_3wcllafbrmtETGGZ0MPPojsDNlHwjc6WH9trhn7-Twg5jQeBqH5JsNIOvw=w1511-h671)



**References**
[Google guidelines](http://developer.android.com/tools/projects/index.html)
[Stackover flow  question](http://stackoverflow.com/questions/16601299/how-to-create-a-library-project-in-android-studio-and-an-application-project-tha)