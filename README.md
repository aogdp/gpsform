#Data Collection using Google Forms & Leaflet

This is a simple web app that uses Google Forms and Leaflet to allow data collection using just a modern web browser. Check out the [demo](https://aogdp.github.io/gpsform/) and start collecting!

![](https://raw.githubusercontent.com/aogdp/gpsform/gh-pages/img/gpsform.png)

##Instructions

1. [Dowload](https://github.com/aogdp/gpsform/archive/gh-pages.zip) the app.
2. Create a Google Form with Latitude (Short answer), Longitude (Short answer) and Description (Paragraph) fields/questions.
3. Connect your form resposnes to a spreadsheet.
4. [Publish](https://support.google.com/docs/answer/37579?hl=en) your response sheet to the web.
5. [Pre-fill](https://support.google.com/docs/answer/160000?hl=en) the form to get the appropriate variables for the app.

The prefilled form will look something like this:
```
https://docs.google.com/forms/d/formId/viewform?entry.field1=39.01&entry.field2=-81.26&entry.field3=description
```
These are the variables you need to change in index.html:
```javascript
 var formId = 'Your Form Id';
 var formLat = 'Longitude id from prefilled form';
 var formLng = 'Latitude id from prefilled form';
 var formText = 'Description id from prefilled form';
 var gsheet = 'sheet id';
```
6. Upload the app to a webserver or just fork this repository and create a gh-pages branch.
7. You may also want to change the meta tags at the beginning of the page to reflect your app.
9. Start Collecting!
 
##Enhancements
Could be added but I wanted to keep this app as simple as possible.

1. Add styling using Awesome Markers, Maki Markers or other plugins.
2. Add search.
3. More basemaps.
5. Layer selector.
6. Figure out a way to collect pictures taken with the device, and push that url to the google sheet. This would take much more coding than is in the initial app. I suggest this be accomplished manually.


