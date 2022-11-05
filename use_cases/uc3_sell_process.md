# Use-Case Specification: Sell Process

# 1. Getting an overview

## 1.1 Brief Description
This use case allows a user to get an overview over all exisitng sessions. From this screen they can select a session and join it ([Join a Session](./uc4_sell_process.md)).

## 1.2 Mockup
![Mockup getting an overview](../mockups/Session_Overview.png)

# 2. Flow of Events

## 2.1 Basic Flow
- User navigates to the dashboard (Dashboard is the main page of our App so it gets displayed after App start automatically)
- User can see a list of all existing sessions

### Activity Diagram
![Activity Diagram](./ActivityDiagramSale.jpg?raw=true)

### Sequence Diagram
![Sequence Diagram](./SequenceDiagramSale2.jpg?raw=true)


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
Total number of story points: 8
