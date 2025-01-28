# HarmoniQ

HarmoniQ is a Spotify-integrated web application that allows users to explore the mood of their favorite albums, create mood-based playlists, and upload them directly to their Spotify account. With HarmoniQ, music lovers can seamlessly connect their emotions to their music library and discover new ways to enjoy their favorite tunes.

---

## Features

### 1. **Connect Your Spotify Account**

Easily link your Spotify account to unlock all the features of HarmoniQ. Once connected, you can:

- Search for albums in your Spotify library.
- Access personalized recommendations.

### 2. **Mood Analysis of Albums**

Search for any album and get detailed insights into its mood. The app analyzes the emotional tone of the album using advanced AI models and Spotify’s track data to provide:

- Mood descriptors (e.g., happy, melancholic, energetic).
- A visual mood profile of the album.

### 3. **Create Mood-Based Playlists**

Craft your own playlists based on a mood of your choice:

- Select songs or albums that fit a specific mood.
- Combine tracks across genres and artists.
- Automatically upload the new playlist to your Spotify account.

### 4. **Discover New Albums**

Use HarmoniQ’s recommendations to find new albums that match your mood or expand your musical taste.

### 5. **Subscription Features**

Unlock premium features with a subscription, powered by Stripe. Subscribers can:

- Access advanced mood analysis.
- Generate unlimited playlists.
- Get exclusive recommendations.

---

## Getting Started

### Prerequisites

- A Spotify account (Free or Premium).
- An internet browser (Google Chrome, Firefox, or similar).

### Installation

1. Clone the HarmoniQ repository:

   ```bash
   git clone https://github.com/andrewpre/harmoniq.git
   ```

2. Navigate to the project directory:
   ```bash
   cd harmoniq
   ```
3. Install the required dependencies:

   ```bash
   npm install

   ```

4. Set up the Spotify Developer API credentials:
   - Create a Spotify Developer account at [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/).
   - Create a new application and note down the Client ID and Client Secret.
   - Add your Redirect URI in the app settings (e.g., `http://localhost:3000/callback`).
   - Create an `.env` file in the root of the project and add:
     ```env
     SPOTIFY_CLIENT_ID=your-client-id
     SPOTIFY_CLIENT_SECRET=your-client-secret
     SPOTIFY_REDIRECT_URI=http://localhost:3000/callback
     STRIPE_SECRET_KEY=your-stripe-secret-key
     SUPABASE_URL=your-supabase-url
     SUPABASE_KEY=your-supabase-key
     ```
5. Start the development server:
   ```bash
   npm run dev
   ```
6. Open the app in your browser at `http://localhost:3000`.

---

## Usage

1. **Log in to Spotify**: Click the "Connect to Spotify" button on the homepage to log in to your account.
2. **Search Albums**: Use the search bar to find albums you want to analyze.
3. **View Mood Analysis**: Explore the mood profile of your favorite albums, displayed with intuitive visualizations.
4. **Create Playlists**: Select songs and create mood-based playlists. Save them to your Spotify account with one click.
5. **Subscribe for More**: Unlock additional features by subscribing through Stripe.
6. **Discover New Music**: Get recommendations based on the mood of the albums you enjoy.

---

## Technologies Used

- **Frontend**: Next.js, Tailwind CSS
- **Backend**: Next.js
- **Database**: Supabase (PostgreSQL)
- **Authentication**: Supabase Auth
- **Payment Integration**: Stripe
- **API Integration**: Spotify Web API
- **Mood Analysis**: AI-based sentiment analysis algorithms

---

Enjoy discovering and creating music with HarmoniQ! 🎶

---
