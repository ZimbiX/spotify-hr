Spotify HR FitBit App
=====================

This is source code for the Spotify HR on the FitBit Versa.

![Demo](https://image.ibb.co/m4UNqy/image.png)

Features
========

The app is a remote controller for your Spotify account.

 - Remote control music playback
 - Change playlist
 - Volume control
 
Why *HR*?
=========

HR stands for Heart-Rate. Spotify HR implements a unique Heart-Rate based shuffle feature.
When enabled the songs in your current playlist will be shuffled to match your current heart rate during playback.
With faster and higher tempo songs being played as your heart rate increases.
A nice addition to enjoy matching music to any varied workout.

![HR Shuffle](https://image.ibb.co/daFFcd/image.png)

Manual installation
===================

Unfortunately, this app hasn't been approved for the Fitbit App Gallery yet. Until then, here's how to manually install it from source yourself:

- If you're not already set up as a Fitbit developer, follow the [Getting Started guide](https://dev.fitbit.com/getting-started/) in order to make an account, create a blank project in Fitbit Studio, and connect up your watch
- [Download the source code of this app](https://github.com/TimeToogo/spotify-hr/archive/master.zip), then extract the archive, and drag the contents into the left panel of your Fitbit Studio project
- You'll need Spotify API credentials, so [register for a Spotify Developer account](https://developer.spotify.com/dashboard/login)
    + Once registered, create a client ID:
        * Enter anything you like in the form that appears
        * Once created, in its settings, set the Redirect URI field to `https://app-settings.fitbitdevelopercontent.com/simple-redirect.html`
- Copy the Client ID and Client Secret into `common/spotify.secret.example.js` in Fitbit Studio and rename the file to remove `.example`
- Make sure the studio's still connected to your watch as it's bound to have timed out by this point
- Click Run to install it to your watch
- In the developer menu of the Fitbit phone app, tap the name of your project, then Settings, to authorise controlling your Spotify account
- If the app isn't working and you see something like `companion stopped` in the studio console, just hit Run again - this is a bug with the platform
- Move it to the first page of apps on your watch for easy access
- Enjoy!
