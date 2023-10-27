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

## Project Screen Shot(s)

[ PRETEND SCREEN SHOT IS HERE ]

[ PRETEND OTHER SCREEN SHOT IS HERE ]

## Installation and Setup Instructions

#### Example:  

Clone down this repository. You will need `node` and `npm` installed globally on your machine.  

Installation:

`npm install`  

To Run Test Suite:  

`npm test`  

To Start Server:

`npm start`  

To Visit App:

`localhost:3000/ideas`  

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
