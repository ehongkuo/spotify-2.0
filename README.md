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

## Reflection

  - What was the context for this project? (ie: was this a side project? was this for Turing? was this for an experiment?)
  - What did you set out to build?
  - Why was this project challenging and therefore a really good learning experience?
  - What were some unexpected obstacles?
  - What tools did you use to implement this project?
      - This might seem obvious because you are IN this codebase, but to all other humans now is the time to talk about why you chose webpack instead of create react app, or D3, or vanilla JS instead of a framework etc. Brag about your choices and justify them here.  

#### Example:  

This was a 3 week long project built during my third module at Turing School of Software and Design. Project goals included using technologies learned up until this point and familiarizing myself with documentation for new features.  

Originally I wanted to build an application that allowed users to pull data from the Twitter API based on what they were interested in, such as 'most tagged users'. I started this process by using the `create-react-app` boilerplate, then adding `react-router-4.0` and `redux`.  

One of the main challenges I ran into was Authentication. This lead me to spend a few days on a research spike into OAuth, Auth0, and two-factor authentication using Firebase or other third parties. Due to project time constraints, I had to table authentication and focus more on data visualization from parts of the API that weren't restricted to authenticated users.

At the end of the day, the technologies implemented in this project are React, React-Router 4.0, Redux, LoDash, D3, and a significant amount of VanillaJS, JSX, and CSS. I chose to use the `create-react-app` boilerplate to minimize initial setup and invest more time in diving into weird technological rabbit holes. In the next iteration I plan on handrolling a `webpack.config.js` file to more fully understand the build process.
