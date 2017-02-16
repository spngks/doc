# Android-Code-Challenge

`challenge status: open`

## What You'll need to build
Write an Android application with a library project (SDK) using Java. Only the library project should make an HTTP GET request to "http://private- d847e-demoresponse.apiary-mock.com/questions"
Once loaded, library project should at least randomly select one object from the response and generate a View/ViewGroup with text or image. Ad d features as you like, use your imagination, but coding standard and overall architecture will have the highest value.
The Library Project should handle the following,
sending the request parsing the response view generation
The Android App,
integrate the library project display the content
Constraints
1. No 3rd party library can be used.
2. No 3rd party app development frameworks can be used ( e.g PhoneGap, etc..)
Bonus Points
At Smaato, we do our best to go the extra mile and as such you would receive bonus points if
1. Let the Library project create the View(s) and Android App display the generated View. 2. Export the Library project as a jar or aapt file.
3. Usage of Unit Testing framework like Robolectric etc.
4. UI testing using UIAutomator / Espresso etc.
Deliverables
1. Android Studio project with source code
2. Integration steps if created a Library jar/aapt and if needed.
API Response Format
A JSON array representing image or text information along with user name and country. The response is NOT case sensitive.
Image Object Format
     
    {
"created": -449280, /* number of seconds passed since created */ "type": "IMG",
"data": { "url": "https://pixabay.com/xxxx"},
"user" : {
"name": "John", "country":"USA" }
}
 Text Object Format
    {
"created": -280800, /* number of seconds passed since created */ "type": "TEXT",
"data": {
"text": "The real danger is not that computers will begin to think like men, but that
men will begin to think like computers."
} "user": {
"name": "Sydney Harris", "country":"USA"
}
}
 Note
Please note that the JSON array might have invalid or incomplete object e.g.
   {
"created": 0
}
 
