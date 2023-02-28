# Using Tasker on Android to Run RICOH THETA Web API Commands automatically

![ricohicon](images/icon/green-logo-96x96.png)
![taskericon](images/icon/android-chrome-96x96.png)
![httpreqicon](images/icon/httpreqshort96.png)
<svg role="img" fill="#3DDC84" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" width="96px" height="96px" ><title>Android</title><path d="M17.523 15.3414c-.5511 0-.9993-.4486-.9993-.9997s.4483-.9993.9993-.9993c.5511 0 .9993.4483.9993.9993.0001.5511-.4482.9997-.9993.9997m-11.046 0c-.5511 0-.9993-.4486-.9993-.9997s.4482-.9993.9993-.9993c.5511 0 .9993.4483.9993.9993 0 .5511-.4483.9997-.9993.9997m11.4045-6.02l1.9973-3.4592a.416.416 0 00-.1521-.5676.416.416 0 00-.5676.1521l-2.0223 3.503C15.5902 8.2439 13.8533 7.8508 12 7.8508s-3.5902.3931-5.1367 1.0989L4.841 5.4467a.4161.4161 0 00-.5677-.1521.4157.4157 0 00-.1521.5676l1.9973 3.4592C2.6889 11.1867.3432 14.6589 0 18.761h24c-.3435-4.1021-2.6892-7.5743-6.1185-9.4396"/></svg>

## You will Learn
* Using the Tasker App to Run RICOH THETA Web API Commands Sequentially
* Sharing your Task with others to use on their device


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

## Resources
* [THETA Web API v2.1](https://github.com/ricohapi/theta-api-specs/tree/main/theta-web-api-v2.1)

## General Steps
1. [Get Deep-linking URL from HTTP Shortcuts app](http-req-tut.md)

2. [Use Tasker App to Run Commands Sequentially](tasker-tut.md)

3. [Add Tasker Commands to Device Home Screen](homescreen-tut.md)

4. [Exporting Task as Link to share with others](export-tut.md)