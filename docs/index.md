# Using Tasker on Android to Run API Commands automatically

![ricohicon](images/icon/green-logo-96x96.png)
![taskericon](images/icon/android-chrome-96x96.png)
![httpreqicon](images/icon/httpreqshort96.png)

## Summary 
Today, I’m going to explain how to test the RICOH THETA X model using the free mobile app [HTTP Request Shortcuts](https://play.google.com/store/apps/details?id=ch.rmy.android.http_shortcuts) and the paid mobile app [Tasker](https://play.google.com/store/apps/details?id=net.dinglisch.android.taskerm&hl=en_US&gl=US) for $3.49. With this combination you are able to take pictures and configure camera settings in the field with a custom workflow using an Android phone or tablet where you may be putting the camera in a car with one hand and holding the phone in your other hand. Similar apps are also available for iOS.

This may be an easy way to prototype workflows specific to the industry you are working in, before doing final development on your app.

To send HTTP Requests with HTTP Request Shortcuts I followed this article [Using the THETA Web API without programming (Remote photo app)](https://community.theta360.guide/t/using-the-theta-web-api-without-programming-remote-photo-app/4796) and if you need further information to reference I have an article testing the RICOH THETA Web API with HTTP Requests Shortcuts here [Testing RICOH THETA Web API via Android Mobile App](https://community.theta360.guide/t/testing-ricoh-theta-web-api-via-android-mobile-app/8797).

Tasker is going to be used to execute a set of API commands automatically from HTTP Request Shortcuts and group them together so we can organize a set of custom API requests into one group and press one button to set them off sequentially. We can also set that group of commands from tasker into a home screen shortcut!

## Camera

    Name: RICOH THETA X
    Firmware: 1.41.0
    
    Reset camera
        Can be done through LCD on camera or using the API
    
    Delete all media on camera
        Can use USB cable, connect to Windows, delete through Windows explorer

## Device connected to Camera

    Device: Samsung Galaxy Tab A8
    Model Name: SM-X200
    Android Version: 13

## Apps Used
* [Tasker](https://play.google.com/store/apps/details?id=net.dinglisch.android.taskerm&hl=en_US&gl=US)
* [HTTP Request Shortcuts](https://play.google.com/store/apps/details?id=ch.rmy.android.http_shortcuts)


## General Steps

1. Get Deep-linking URL from HTTP Shortcuts app

2. Use Tasker App to Run Commands Sequentially

3. Add Tasker Commands to Device Home Screen

4. Exporting Task as Link to share with others