## Spotify 2.0

#### Click here to view: [spotify-2](https://spotify-2-zeta.vercel.app/)
![Preview](/assets/images/preview.png)


Spotify 2.0 is an application that mirrors the Spotify app, designed to look and function like Spotify. While the goal of this project was to make as close of a copy as possible, that is a very challenging task. Current features include:

- Song upload
- Play song audio
- Favorites system
- Playlists / Liked songs system
- Play/Pause, Skip forward/backwards
- Volume Control
- Premium Subscription with Stripe (Necessary for functionality, instructions below)

The technologies/technical features involved in this project include:

- __React.js__:
  - Components, hooks, and state widely used throughout project
  - react-hook-form: form client form validation and handling
  - react-toast: server error handling/notifications
- __Next.js__:
  - React functionality integrated with Vercel
  - seamless deployment/build structure
- __Tailwind__:
  - CSS framework for sleek UI
  - animations/transition effects
  - full responsiveness for all devices
- __Supabase__:
  - PostgreSQL Database handling
  - credential authentication
  - file and image upload
  - data fetch from components with client
  - Global songs library and account-specific settings/data
- __Stripe__:
  - API to handle subscriptions and payment
  - 

## Setup Instructions

First, you need to visit the website that is deployed using Vercel. If the above link does not work, try using this url: [https://spotify-2-zeta.vercel.app/](https://spotify-2-zeta.vercel.app/)

Once you have entered the website, you will notice that there are a couple songs already displayed. You will also be able to navigate to the app's liked songs, search page, or return home using the corresponding buttons. The songs that you see are songs that I uploaded during development or songs other users uploaded! If you try clicking on them, first you will notice that you are unable to play the song as it will ask you to log in. In fact, no matter which song or location you try, the app requires that you log in before you can listen. Don't worry, making an account is free! You should see this page:

![auth modal](/assets/images/auth_modal.png)

Once you create an account and verify your email, you should be logged in! You will see the following in the corner of the page instead of the "log in/sign up" buttons:

![logged_in](/assets/images/premium.png)

However, you will still be unable to play songs because you are not yet subscribed! Don't worry, for this project and app, the subscription is only there for the sake of integrating stripe, you can use a test card to get a subscription for free! Heres how:

First click on the "Subscribe for $9 a month" button

![premium_only](/assets/images/premium_only.png)

This link will take you to a stripe link that looks like this:

![stripe](/assets/images/stripe.png)

Here you will need to enter card information but since this app is using stripe in test mode, as denoted in orange, you can use the the test number __4242 4242 4242 4242__ to get a free premium subscription! For the rest of the information such as CVV and address, you can put whatever you like, it doesn't matter!

![test_card](/assets/images/test_card.png)

Once you are subscribed, it will take you back to your accounts page and it should look like this, denoting that your subscription went through:

![success](/assets/images/success.png)

Now, you are finally able to use this app to its full capacity! Feel free to try uploading songs, playing them, liking them and searching for them in the search page!
Thanks and hope you have a good time!

## Reflection (Q&A Format)

  - __Q: What was the context for this project?__
  - A: This project was something I decided to work on because Spotify has many features that initially seemed to have intuitive applications for CS fundamentals such as DS and algorithms. Playlists -> Arrays/Queues, Songs -> OOP, etc. Also, music is a passion of mine and I loved the idea of using software to create something related to it.
    
  - __Q: Why was this project challenging and therefore a really good learning experience?__
  - A: This project's greatest challenge so far was, _surprisingly_, implementing basic playlist functionalities. Although songs were playing correctly, playlists of songs and skip/replay functions would not behave correctly for some time. Features that initially seemed to only require basic arrays, loops, and conditionals to implement quickly became a large mess of issues that eventually pointed to a core issue: compatibility with the “use-sound” library that was necessary to play songs. Eventually, I ended up designing the Player so that it would manually re-render a new instance of a Player for each song. While performance is not optimal, I prioritized getting a working application and optimizations are a current challenge in the works. All in all, definitely has been a great learning experience so far.
  
  - __Q: What have you learned from this project?__
  - A: This project taught me that focusing too hard on features or optimizations can be unproductive when losing sight of the larger goal. Moving on from especially challenging problems without optimization led to greater productivity because it allowed me to complete a working application. This project also taught me how to find working solutions while facing core design issues.
    
  - __Q: What are some future features you hope to implement?__
  - A: Dynamic Song loading (maybe by pre-rendering the next song before the current one finishes, or employing a new song player library), Global volume state, Multiple playlists/Playlist folders, and Shuffle are a few on my mind. These features will be added and published in this repository as they are completed.
