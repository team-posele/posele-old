# Posele

by Luke Joo, Smit Patel, John Arroyo, and Tyler Monaghan

## Requirements

_'user' refers to a logged-in user unless otherwise specified_

### **Tier 0: MVP**

  <details>

**user experience**

- [ ] Users can open our app on up-to-date iPhone or Android device
- [ ] Users can Sign Up for an account by providing an email address and password
- [ ] Users can Log In to the app by providing their email address and/or username and password
- [ ] Users can select a PLAY button to play a randomly selected posele
- [ ] A **guest** can play a trial with a single posele
- [ ] Users can see their "score"
  - [ ] how many posele's they have successfully matched out of 5
  - [ ] users score persists and will display on log-in even if they leave or logout of the app

**engineering requirements**

- [ ] Five 'poseles' hosted through Firebase. Each posele consists of an image and a ML model that
      is trained to recognize the posture/pose of the image subject.
- [ ] Create a machine learning model for each posele
- [ ] Train the model with our own poses.
- [ ] Users authenticate via Firebase
- [ ] User database model is established in Firebase

**gameplay**

_When a user presses play to begin a posele:_

- [ ] User is provided instructions and prompted to be sure they are in a space where they can move
      and take photographs safely
- [ ] User is presented with an image
- [ ] User presses READY button
- [ ] User device camera opens; photograph is captured after 5 second countdown
- [ ] User is taken to a screen telling them whether they matched the posele (pass/fail)

  </details>

### **Tier 1**

<details>

**user experience**

- [ ] As a user,
- [ ] A guest:
- [ ] Can’t view global leader board, or anonymized
- [ ] Global leader board: can view your score and others’ scores
- [ ] Screenshot/share your score
- [ ] User can select new gameplay option: multi-user party mode (local)

**engineering requirements**

**gameplay**

_Users can now select a new game mode: local hot-phone multiplayer ("party mode")_

- [ ] User will be prompted to select a number of players
- [ ] Instructions will appear on screen (players should complete one posele then pass the phone)
- [ ] The game will rapidly display a posele for each player with a short delay and message to PASS
      the device between each
- [ ] After all poseles are complete, show a scoreboard showing the results for each player

  </details>

### **Tier 2**

<details>

**user experience**

- [ ] Daily limit - can only attempt one posele per day
  - [ ] accounts marked as admin can ignore this limit and play over and over
- [ ] Users can share link to specific pose/share their results after completing a posele
- [ ] Friends: Users can mark other players on the leaderboard as "Friends"
- [ ] Users can filter leaderboard to show only friends
- [ ] Share username
- [ ] Add/remove friends by username
- [ ] Each user friends list
- [ ] Friends private leader board

**engineering requirements**

- [ ] database model must have a way of indicating whether an account has admin permissions
- [ ] players who are not admin can't access poseles other than the current daily posele

</details>

### **Tier ∞**

<details>

**user experience**

- [ ] Additional user stats and metrics available, e.g:
  - [ ] % of users who successfully completed this posele
  - [ ] current streak of correct poseles
  - [ ] current daily streak
- [ ] Display POSEle rank
- [ ] Subscription to allow users to send us money
- [ ] User can select to receive daily push notification reminders of daily posele at select time
- [ ] User can receive push notifications alerting them that a friend has shared or completed a
      posele
- [ ] New gameplay mode: Synchronous game experience
- [ ] Share pose improvements:
  - [ ] Share button redirects to social networking site with pre-formed post including screenshot
        and link
- [ ] Link to the same pose the user attempted (from outside of app)
- [ ] Practice mode: play without a timer to understand the game mechanics without time pressure
- [ ] Camera overlay: the partially-transparent image source is overlaid over the camera preview
      when counting down to take posele photo
- [ ] Choose difficulty (easy vs hard)
- [ ] Post to Instagram/Twitter

**gameplay**

- [ ] new gameplay mode: remote synchronous multiplayer ("BYOD" party mode)

  - [ ] one user starts the app and selects this option, then "host"
  - [ ] user is provided with a short code to share with friends
  - [ ] friends start the app and select this option, then "join"
  - [ ] friends each enter the key and are joined to the host lobby
  - [ ] once all players have joined, host can press Play
  - [ ] all players play the same single posele simultaneously. Hijinks ensue

- [ ] altering difficulty changes the selection of poseles available and time limit

**engineering requirements**

- [ ] Admin panel - admin users can access backend and add/edit/delete users, poseles, and
      leaderboards via the app or a web portal
- [ ] Add license

  </details>
