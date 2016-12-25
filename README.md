# Interview-Practice
This is a “dry-run” interview that simulates an in-person interview. The "dry-run" interview will consist of a series of questions that should be answered within a 1 hour time limit. One may add images where applicable to simulate any "whiteboard" drawings.


1- What’s your favorite tool or library for Android? Why is it so useful?

Butterknife simply to reduce boilerplate code in my application by inject views (or setting click listeners). It's fast, small in size and straightforward in use. It's intended to inject views, listeners and other UI related objects.


2- You want to open a map app from an app that you’re building. The address, city, state, and ZIP code are provided by the user. What steps are involved in sending that data to a map app?

The Google Maps app for Android exposes several intents that i can use to launch Google Maps in display, search, navigation, or Street View modes. 

That encourage me to use intent after creating the Intent, i can request that the system launch the related app in a number of ways. A common method is to pass the Intent to the startActivity() method. The system will launch the necessary app — in this case Google Maps — and start the corresponding


Steps :
Create a Uri from an intent string.
Create an Intent from gmmIntentUri. Set the action to ACTION_VIEW.
Make the Intent explicit by setting the Google Maps package.
Attempt to start an activity that can handle the Intent.


3- Implement a method to perform basic string compression using the counts of repeated characters. For example, the string aabcccccaaa would become a2b1c5a3. If the "compressed" string would not become smaller than the original string, your method should return the original string. The method signature is: “public static String compress(String input)” You must write all code in proper Java, and please include import statements for any libraries you use.

Here is my implementation






4- List and explain the differences between four different options you have for saving data while making an Android app. Pick one, and explain (without code) how you would implement it.
Shared Preferences : Store private primitive data in key-value pairs.
Internal Storage : Store private data on the device memory.
External Storage : Store public data on the shared external storage.
SQLite Databases : Store structured data in a private database.
Network Connection : Store data on the web with your own network server.
Shared Preferences
The SharedPreferences class provides a general framework that allows you to save and retrieve persistent key-value pairs of primitive data types.

To write values: 
Call edit() to get a SharedPreferences.Editor.
Add values with methods such as putBoolean() and putString(). 
Commit the new values with commit() 
To read values, use SharedPreferences methods such as getBoolean() and getString().



5- What are your thoughts about Fragments? Do you like or hate them? Why?

My thought: Imagine Activity as a plate that hold one big cake. Fragment would be a container that slices the same cake into pieces. Each slice contains it own logics (listeners, etc). And in total they are almost no different with the one big cake. 

I like Fragments because: 
When you plate can't hold a big cake. (Screen is small) You can easily use a a few plates (Activity) to hold each of them WITHOUT the need to move your logics into the new activity. Better re-usability.

I have some instances where I could reuse a fragment entirely in another App. You might claim that a custom view could does that too. But refer to point 1, I could reuse it with just few lines of layout changes but for a custom view, it have to find a way to plug it into both layout and code. It is, in some sense, a more OO ways of organising your UI logics in Android programming. 

When you have a feature (A new partition on the screen for example), you create a new Fragment class, with minor modification to existing activity class. However if you are programming only with activity, you will need to add logics and make big modification on tested class.

6- If you were to start your Android position today, what would be your goals a year from now?

By next year, I want to see myself leading a team or android developers, building something cool. I also have plans to contribute more towards open source software and help the Android community make great products.
