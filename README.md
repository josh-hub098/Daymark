# To-Do + Habit Tracker

A responsive daily dashboard for tasks, habits, streaks, and completion progress. It has no build step or external dependencies.

## Run

Open [Daymark](https://josh-hub098.github.io/Daymark/) on the web, or open `index.html` in a browser for local use. Profiles and tracker data are stored in that browser on that device.

## Install on PC or mobile

To install Daymark as an app and use it offline, publish all project files together on a static web host that serves HTTPS, then open that address on each device:

- On desktop Chrome or Edge, choose **Install** from the browser menu or address bar.
- On Android, open the address in Chrome and choose **Install app** or **Add to Home screen**.
- On iPhone, open the address in Safari, tap **Share**, then **Add to Home Screen**.

The offline cache is saved after the first online visit. Each device keeps its own profiles and data; there is no cloud account or sync. Opening `index.html` directly still works, but browser installation and offline caching require HTTPS (or localhost).

## Offline profiles and notifications

- Passwords are stored as salted PBKDF2 hashes. This local sign-in is a convenience gate, not server-backed authentication or encrypted storage; use a password unique to this app.
- Password reset compares the username and phone number saved on this device. It does not send an SMS or independently verify identity.
- Task reminders and quote notifications can appear while Daymark is open. Allow browser notifications in Settings for system alerts. A fully closed offline app cannot send scheduled notifications; that requires a push service.

## Features

- Add, complete, and delete tasks
- Add, check in to, and delete daily habits
- Track consecutive habit streaks
- See daily completion percentage and a seven-day habit rhythm
- Review current progress in the Insights view

Data stays in the current browser and is not synced between devices.
