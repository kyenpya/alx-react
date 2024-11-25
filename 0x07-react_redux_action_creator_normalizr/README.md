# React Redux Action Creators and Normalizr Project

This project focuses on understanding and implementing React Redux concepts, including action creators, state normalization using Normalizr, and testing Redux functionalities. Below are the details and structure for the project.

## Tasks

### Task 0: Read Data from JSON
-Objective: Create a function `getAllNotificationsByUser` in `notifications.js` that filters notifications by `userId`.
-Test: Verify output matches the provided sample data using Jest.


### Task 1: Normalize a Nested JSON
-Objective: Use Normalizr to set up entities for `users`, `messages`, and `notifications`.
-Test: Validate normalized data structure for `result`, `users`, `messages`, and `notifications`.


### Task 2: Filter a Normalized Schema
-Objective: Refactor `getAllNotificationsByUser` to use normalized data.
-Requirement: Minimize looping and ensure existing tests pass.


### Task 3: Create Actions for Course List
-Action Types:
  -`SELECT_COURSE`
  -`UNSELECT_COURSE`
-Action Creators**:
  -`selectCourse(index)`
  -`unSelectCourse(index)`
- Test: Validate action creators using Jest.


### Task 4: Create Actions for UI
-Action Types:
  -`LOGIN`, `LOGOUT`
  -`DISPLAY_NOTIFICATION_DRAWER`, `HIDE_NOTIFICATION_DRAWER`
-Action Creators:
  -`login(email, password)`
  -`logout()`
  -`displayNotificationDrawer()`
  -`hideNotificationDrawer()`
-Test: Write unit tests for all action creators.


### Task 5: Create Actions for Notifications
-Action Types:
  -`MARK_AS_READ`
  -`SET_TYPE_FILTER`
-Filters: 
  -`NotificationTypeFilters = { DEFAULT, URGENT }`
- Action Creators:
  -`markAsRead(index)`
  -`setNotificationFilter(filter)`
- Test: Verify actions with Jest.


### Task 6: Bind the Actions
- Modify all action creators to bind them appropriately:
  - Course, Notification, and UI actions.


### Task 7: Async Action Creators
- Setup:
  - Install `redux` and `redux-thunk`.
  - Simulate an API using `login-success.json` and `notifications.json`.
- Action Types:
  - `LOGIN_SUCCESS`
  - `LOGIN_FAILURE`
- Action Creators:
  - `loginSuccess()`
  - `loginFailure()`
  - `loginRequest(email, password)`
- Test: Use `redux-mock-store` and `fetch-mock` to simulate API interactions.


## How to Run
1. Clone the repository.
2. Navigate to the task directory.
3. Install dependencies using `npm install`.
4. Run tests using `npm test`.