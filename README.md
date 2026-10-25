# CS-360-Mobile-Architecture-Programming

## Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?

The goal of the Event Tracking app was to create a simple mobile app that allows users to login/create an account, create, edit, and delete upcoming events. Events would be displayed to users in a grid-based structure and users could opt in to receive SMS notifications when an event is within 24 hours of it's start time. When creating events, users input a name, date, time, and description (optional) for the event. This app was designed to for people who needed a simple, lightweight app to keep track of their upcoming plans.

## What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?

The app featured 4 unique screens. The login/account creation screen allowed users to create and login accounts so that events are stored within their respective accounts. This feature was useful if multiple users had access to the device or the accounts were used as another way for the user to sort their events. The SMS Permission screen prompted the user if they wanted to opt in to SMS notifications. If they declined, the app would still function as normal, just without the reminders. The events screen allowed users to view their events. Events were sorted from soonest to latest with headers for each date and the name and time of each event listed in their own cards. A new event can be created using the floating action button at the bottom right of the screen. Users can also delete and edit events using the respective buttons on an event card. Tapping the event card itself will also show users the description for that event if one exists. Finally, the event creation screen allows the users to input a name, date, time, and description for the event. When inputting a date, a date picker is used to let the user select a date while the time picker lets users select a time for the event. If the user enters this screen using the edit button, the screen will be filled out with existing information. I believe my designs were a successful overall, but lacks polish.

## How did you approach the process of coding your app? What techniques or strategies did you use? How could those techniques or strategies be applied in the future?

When approaching the process of coding my app, I broke down the app into smaller components that I could work on. This allowed me to better focus on specific component I was working on and mitigated wondering onto other aspects of the app. One technique that I utilized was creating Helper classes. These classes were created to reduce duplicate code and better streamline the work process. For example, I created a Database Helper class that handles the database for both the accounts and the events. This strategy will be very helpful in the feature because breaking down problems into smaller parts can make them easier to understand. 

## How did you test to ensure your code was functional? Why is this process important, and what did it reveal?

When testing my code to ensure functionality. I tested the app on the supported versions of android as well as thoroughly testing the functionality of each feature. This process is important because apps are typically built with multiple android versions in mind rather than just the latest. If you plan to support older versions, then you need to test on those versions as well. Failure to test on older, supported versions can result in unintended bugs.

## Consider the full app design and development process from initial planning to finalization. Where did you have to innovate to overcome a challenge?

One place that I had to innovate to overcome a challenge was the SMS requirement. Since I had no knowledge of mobile app development, I thought I would just have a card pop-up asking for permission. This changed into an SMS permission screen later on because I needed to allow the user to turn off and on the notifications whenever they wanted to.

## In what specific component of your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?

The component that I was particularly success in demonstrating my knowledge was the database and the data-handling. The app has user and event tables, account creation and login logic, and has all CRUD operations all separated into their own classes. These classes supports multiple aspects of the app from login to event creation. Each account has their own event table and editing events has their parameters prefilled.
