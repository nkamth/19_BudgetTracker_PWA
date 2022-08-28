# 19_BudgetTracker_PWA

- Using Progressive Web Application (PWA) this application enables the user to add expenses and deposits to their budget with or without an online connection. When entering transactions offline, data should populate the total when connected back online.
- Launch the application <a href="https://budgetracker10.herokuapp.com/" target="_blank"> > https://budgetracker10.herokuapp.com/ < </a>

![](public/img/sample.PNG)

### User Story

AS AN avid traveller
I WANT to be able to track my withdrawals and deposits with or without a data/internet connection
SO THAT my account balance is accurate when I am traveling

### Business Context

Giving users a fast and easy way to track their money is important, but allowing them to access that information anytime is even more important. Having offline functionality is paramount to our applications success.

## Table of contents

- [General Info](#Info)
- [Functionality](#Functionality)
- [Install](#Install)
- [Dependencies](#Dependencies)
- [Technologies](#Technologies)
- [Github Repo Linl](#Github)
- [Deployed URL](#Deployed)
- [Contact](#Contact)

# General Info

### What is Progressive Web Application (PWA)?

- A Progressive Web App (PWA) is a web app that uses modern web capabilities to deliver an app-like experience to users. These apps meet certain requirements (see below), are deployed to servers, accessible through URLs, and indexed by search engines.

### What is required for PWA?

To be considered a Progressive Web App, your app must be:

- Progressive - Work for every user, regardless of browser choice, because they are built with progressive enhancement as a core tenet.

- Responsive - Fit any form factor, desktop, mobile, tablet, or whatever is next.

- Connectivity independent - Enhanced with service workers to work offline or on low quality networks.

- App-like - Use the app-shell model to provide app-style navigation and interactions.

- Fresh - Always up-to-date thanks to the service worker update process.

- Safe - Served via HTTPS to prevent snooping and ensure content has not been tampered with.

- Discoverable - Are identifiable as “applications” thanks to W3C manifests and service worker registration scope allowing search engines to find them.

- Re-engageable - Make re-engagement easy through features like push notifications.

- Installable - Allow users to “keep” apps they find most useful on their home screen without the hassle of an app store.

- Linkable - Easily share via URL and not require complex installation.

#### Offline Support

- Apps should be able to work offline. Whether that be displaying a proper "offline" message or caching app data for display purpose.

# Functionality

BUDGET-TRACKER Offline Functionality:

- Enter deposits offline
- Enter expenses offline

When brought back online:

- Offline entries should be added to tracker.

## _In order to achieve OFFLINE SUPPORT, a manifest file and a service worker file must be created._

### Manifest `manifest.webmanifest`

- #### Purpose
  - The manifest file is a simple text file (JSON file) that lists the resources (app's displayed name, icons, as well as splash screen) the browser should cache for offline access.

### Service Worker `service-worker.js`

- #### Purpose

  - Service worker provides a programmatic way to cache app resources.

- #### Service Worker Life Cycle
  - install
  - activate
  - fetch

# Install

```bash
npm i install

npm i express

npm i mongoose

```

### Run

- 1. Install all dependencies (see above)
- 2. Create a terminal on the Budget-Tracker folder and run:
  ```bash
  mongod
  ```
- 3. Create another terminal on the same folder and run:

  ```bash
  node server
  ```

- 4. Deploy it to heroku

# Dependencies

```bash
"dependencies": {
    "express": "^4.17.1",
    "install": "^0.13.0",
    "mongodb": "^3.5.5",
    "mongoose": "^5.9.7",
    "nodemon": "^2.0.2"
  }

```

# Technologies

- HTML5
- CSS
- jQuery
- Express
- MongoDB
- Mongoose
- IndexedDB
- Bootstrap

# Github Repo Link

https://github.com/nkamth/19_BudgetTracker_PWA

# Deployed URL

https://budgetracker10.herokuapp.com/

# Contact

- Namitha V Kamath
- github: https://github.com/nkamth
- email: namitha.289@gmail.com
