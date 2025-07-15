#  Movie Finder App 

A sleek React-based movie search and discovery app powered by the [TMDB API](https://developer.themoviedb.org/). Users can search for movies, see trending picks, and view posters — all in real-time.

---

## Features

-  **Search Movies** – Find movies by name using TMDB’s `/search/movie` endpoint  
-  **Trending Movies** – Shows a custom trending section based on what users search  
-  **Detailed Movie Cards** – Displays poster, title, and other metadata  
-  **Debounced Input** – Reduces API calls while typing  

---

## Tech Stack

- **Frontend**: React + Vite  
- **Styling**: Tailwind CSS / Custom CSS  
- **Data Source**: [TMDB API](https://developer.themoviedb.org/)  
- **Optional Backend**: [Appwrite](https://appwrite.io/) for trending analytics  

---

## How Appwrite Powers the Trending Section

While TMDB provides globally popular movies, this app uses **Appwrite** to build a **custom trending system** based on **user searches**.

###  How it works:

Every time a user searches for a movie, we store or update a document in Appwrite.

We track:

- How many times a movie has been searched  
- When it was last searched  
- Its poster, title, TMDB ID, etc.  

The **Trending** section then shows the movies with the highest `search_count`.


you can view it [here](https://movie-app-r128.vercel.app/)

