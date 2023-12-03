# **Meet App**

### **Objective :**
_To build a serverless, progressive web application (PWA) with React using a
test-driven development (TDD) technique. The application uses the Google
Calendar API to fetch upcoming events._

[Meet App hosted on Github Pages](https://mattsperez.github.io/meet/)

### **Feature User Stores:**

Feature 2: Show/Hide Event Details

  Scenario 1: Event element is collapsed by default
    Given the user opens the events app
    When they view an event element
    Then the event details should be collapsed

Scenario 2: User can expand an event to see details
    Given the user is viewing an event element
    When they click on the expand button or tap on the event
    Then the event details should be visible
    And the expand button should change to a collapse button

Scenario 3: User can collapse an event to hide details
    Given the user is viewing an expanded event with visible details
    When they click on the collapse button or tap on the event
    Then the event details should be hidden
    And the collapse button should change to an expand button

Feature 3: Specify Number of Events

  Scenario 1: Default number of events when the user hasn’t specified a number
    Given the user is on the events page
    When they haven't specified a number of events to display
    Then 32 events should be shown by default

  Scenario 2: User can change the number of events displayed
    Given the user is on the events page
    When they specify a new number of events to display, for example, 20
    Then the events page should refresh
    And 20 events should be displayed on the page

Feature 4: Use the App When Offline

  Scenario 1: Show cached data when there's no internet connection
    Given the user has previously accessed the app and data has been cached
    When the user tries to use the app without an internet connection
    Then the app should display the cached data
    And provide appropriate feedback about the offline mode

  Scenario 2: Show error when user changes search settings (city, number of events) offline
    Given the user has previously accessed the app and data has been cached
    And the app is currently in offline mode
    When the user attempts to change search settings such as city or number of events
    Then the app should display an error message
    And the search settings should not be updated

Feature 5: Add an App Shortcut to the Home Screen

  Scenario 1: User can install the meet app as a shortcut on their device home screen
    Given the user has the meet app installed on their device
    When they access the app and choose to add a shortcut to the home screen
    Then the app shortcut should be successfully added to the device home screen
    And the user should be able to launch the app from the shortcut

Feature 6: Display Charts Visualizing Event Details

  Scenario 1: Show a chart with the number of upcoming events in each city
    Given the user has accessed the event details section of the app
    When they view the chart displaying the number of upcoming events in each city
    Then the chart should be visible and populated with relevant data
    And the user should be able to interpret the distribution of events across different cities

