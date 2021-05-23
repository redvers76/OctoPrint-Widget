Version 1.0 of OctoPrint Widget
(C) K.Fairhurst 2021
v1.0   Initial Release

Following configuration items are used to determine how the widget will work

Create a DAKBoard user in OctoPrint, with read only permissions
Then create an application key for this user
This will be used to authenticate the requests to the API 


The DAKBoard server that hosts your widget needs to be able to access the computer running OctoPrint
As such it cannot be an "internal network" URL that you use, rather one that can be accessed remotely
Use a dynamic DNS service to ensure your IP address is continually updated, or use your external IP address


Because the DAKBoard service uses HTTPS, we need to use HTTPS to ensure that the content can be included
Whether or not you use port 443 externally is up to you,
This external port will need to be forwarded to port 443 of the computer running OctoPrint
You also need to ensure that you have an appropriate certificate installed otherwise the widget might not load
