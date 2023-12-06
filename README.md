# **Meet App**

### **Objective :**
_To build a serverless, progressive web application (PWA) with React using a
test-driven development (TDD) technique. The application uses the Google
Calendar API to fetch upcoming events._

[Meet App hosted on Github Pages](https://mattsperez.github.io/meet/)

### **Feature User Stores:**

**Feature 2:** _Show/Hide Event Details_

 + **Scenario 1:** _Event element is collapsed by default_
   + **Given** _the user opens the events app_
   + **When** _they view an event element_
   + **Then** _the event details should be collapsed_

+ **Scenario 2:** _User can expand an event to see details_
   + **Given** _the user is viewing an event element_
   + **When** _they click on the expand button or tap on the event_
   + **Then** _the event details should be visible and the expand button should change to a collapse button_

+ **Scenario 3:** _User can collapse an event to hide details_
   + **Given** _the user is viewing an expanded event with visible details_
   + **When** _they click on the collapse button or tap on the event_
   + **Then** _the event details should be hidden and the collapse button should change to an expand button_

**Feature 3:** _Specify Number of Events_

 + **Scenario 1:** _Default number of events when the user hasn’t specified a number_
   + **Given** _the user is on the events page_
   + **When** _they haven't specified a number of events to display_
   + **Then** _32 events should be shown by default_

 + **Scenario 2:** _User can change the number of events displayed_
   + **Given** _the user is on the events page_
   + **When** _they specify a new number of events to display, for example, 20_
   + **Then** _the events page should refresh and 20 events should be displayed on the page_

**Feature 4:** _Use the App When Offline_

 + **Scenario 1:** _Show cached data when there's no internet connection_
   + **Given** _the user has previously accessed the app and data has been cached_
   + **When** _the user tries to use the app without an internet connection_
   + **Then** _the app should display the cached data and provide appropriate feedback about the offline mode_

 + **Scenario 2:** _Show error when user changes search settings (city, number of events) offline_
   + **Given** _the user has previously accessed the app and data has been cached and the app is currently in offline mode_
   + **When** _the user attempts to change search settings such as city or number of events_
   + **Then** _the app should display an error message and the search settings should not be updated_

**Feature 5:** _Add an App Shortcut to the Home Screen_

 + **Scenario 1:** _User can install the meet app as a shortcut on their device home screen_
   + **Given** _the user has the meet app installed on their device_
   + **When** _they access the app and choose to add a shortcut to the home screen_
   + **Then** _the app shortcut should be successfully added to the device home screen and the user should be able to launch the app from the shortcut_

**Feature 6:** _Display Charts Visualizing Event Details_

 + **Scenario 1:** _Show a chart with the number of upcoming events in each city_
   + **Given** _the user has accessed the event details section of the app_
   + **When** _they view the chart displaying the number of upcoming events in each city_
   + **Then** _the chart should be visible and populated with relevant data and the user should be able to interpret the distribution of events across different cities_

### **Meet Serverless**

The Meet app utilizes serverless functions for on-demand processing and scalability in features like event filtering and chart generation. This approach ensures flexibility and cost-effectiveness in handling variable loads, allowing the app to prioritize a smooth user experience without managing complex server infrastructures. Leveraging cloud-based serverless solutions enables efficient delivery of real-time event data and chart insights while minimizing operational overhead. The serverless architecture dynamically scales resources, ensuring optimal performance during high-traffic periods.
