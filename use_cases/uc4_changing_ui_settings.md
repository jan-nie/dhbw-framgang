# Use-Case Specification: Changing UI settings

# 1. Getting an overview

## 1.1 Brief Description
The company administrator has the possibility to change the colour palette of the UI for the company. He also has the possibility to add the logo of the company to the UI and thus personalise the IMSE.

## 1.2 Mockup
<img src="mockup_usecase4.png" alt="Screenshot changing UI settings" width="300"/>

## 1.3 Screenshot
see 1.2

# 2. Flow of Events

## 2.1 Basic Flow
- User navigates to the dashboard (Dashboard is the main page of our App so it gets displayed after App start automatically)
- User can see a list of all existing sessions

### Activity Diagram
![Activity Diagram](../activity_diagrams/UCD3_Session_Overview.png)

### .feature File
[.feature File Session Overview](../../frontend/app/src/androidTest/assets/features/UC3_Session_Overview.feature)
```Cucumber
Feature: Use Case 3 Session Overview
    As a USER
    I want to open the app and navigate to the Session Overview page
    On this page I want to see a full overview of all currently available sessions
    Also I want to see detailed information about the Sessions

  @sessionoverview-feature
  Scenario Outline: I want to see all current active Sessions
    Given I open the App
    When I open the Session Overview page
    Then The page should list all the current active Sessions
    And For each Session should the title <title> be shown
    And For each Session should the game <game> be shown
    And For each Session should the place <place> be shown
    And For each Session should the date <date> be shown
    And For each Session should the players count "<numberOfPlayers>" be shown

    Examples:
      | title   | game         | place         | date        | numberOfPlayers   |
      |  Raid   | Wow          |  online       |  01.11.2018 |  10               |
      |  Mario  | Mario Party  |  online       |  07.07.2018 |  30               |
      | Fortnite| Battle       |  online       |  25.09.2018 |  40               |
```

## 2.2 Alternative Flows
n/a

# 3. Special Requirements
n/a

# 4. Preconditions
The Preconditions for this use case are:
1. The user has started the App
2. The user has navigated to the dashboard (after the startup the dashboard is per default the displayed page)
3. At least one sessions was alredy posted

# 5. Postconditions
n/a

### 5.1 Save changes / Sync with server
The displayed data should be updated whenever the user enters the dashboard again or when the user refreshes the page manually.

# 6. Function Points
![Function Points UC3_Session_Overview](../function_points/UC3_Overview.png)
<img src="../function_points/Blue_print.png" alt="Function Points Blue_Print" width="500"/>

Total number of function points: 9.52
