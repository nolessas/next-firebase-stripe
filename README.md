# Registruokis

A client registration system with Firebase authentication and Stripe payment integration.

## Setup Instructions

### Prerequisites
- Node.js and npm installed
- Firebase account (Blaze plan required for external API calls)
- Stripe account

### Initial Setup

1. **Install dependencies**
   ```
   npm install
   ```

2. **Firebase Setup**
   - Create a Firebase project at [firebase.google.com](https://firebase.google.com)
   - Enable Authentication (GitHub, Email/Password, etc.)
   - Create a Firestore database
   - Upgrade to the Blaze plan to enable external API calls
   - Get your Firebase configuration from Project Settings > Your Apps

3. **Stripe Setup**
   - Create a Stripe account
   - Get your API keys from the Stripe Dashboard
   - Create a subscription product

4. **Environment Variables**
   - Copy `.env.local.example` to `.env.local`
   - Fill in your Firebase and Stripe credentials

5. **Deploy Firebase Rules**
   ```
   firebase login
   firebase deploy --only firestore:rules,storage:rules
   ```

6. **Start the development server**
   ```
   npm run dev
   ```

## Features

- User authentication with Firebase
- Subscription payment system with Stripe
- Premium content gating
- User profile management

## Project Structure

- `/components` - React components
- `/firebase` - Firebase configuration and utilities
- `/pages` - Next.js pages
- `/stripe` - Stripe integration utilities
- `/public` - Static assets

## Deployment

```
npm run build
firebase deploy
```

# Next Firebase Stripe 🔥🦓

A demonstration repository of how to set up a subscription payment system using:

- Next.JS
- Firebase
- Stripe

## How to use this Repo

Please see the **blog post** of how this repository works, here:

[Blog Post](https://blog.jarrodwatts.com/set-up-subscription-payments-with-stripe-using-firebase-and-nextjs)

## Thank You!

Thanks for supporting my content.

Consider starring the repo if you like it, and check out my other socials:

[![YouTube Channel Subscribers](https://img.shields.io/youtube/channel/subscribers/UCJae_agpt9S3qwWNED0KHcQ?label=YouTube%20Subscribers!&style=social)](https://www.youtube.com/channel/UCJae_agpt9S3qwWNED0KHcQ?sub_confirmation=1)
[![Twitter Followers](https://img.shields.io/twitter/follow/jarrodwattsdev?label=Twitter%20Followers!&style=social)](https://twitter.com/intent/follow?screen_name=jarrodwattsdev)
