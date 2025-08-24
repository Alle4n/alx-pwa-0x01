# ALX Project 0x14 – Movie App (CineSeek)

This project is a Next.js-based movie application that consumes the **MoviesDatabase API** from RapidAPI.  
Users can browse, search, and filter movies by year and genre, with a clean, responsive UI.

---

## API Overview

The **MoviesDatabase API** provides programmatic access to a large collection of movies and TV series data.  
It supports queries for titles, genres, images, and release years, making it ideal for building movie search and discovery applications.

**Key Features:**
- Search for movies or TV series by keyword.
- Filter results by year, genre, or title type.
- Retrieve detailed metadata such as posters, release year, and title text.
- Paginate through results for large datasets.

---

## Version

`v1` – as provided by RapidAPI.

---

## Available Endpoints

| Endpoint | Description |
|----------|-------------|
| `/titles` | Retrieve a list of movies or TV series, with optional filters (year, genre, title type, pagination). |
| `/titles/search/title/{title}` | Search for titles by exact or partial title text. |
| `/titles/{id}` | Get detailed information about a single movie or TV show by its ID. |
| `/titles/utils/genres` | Retrieve a list of all available genres. |
| `/titles/utils/titleTypes` | Retrieve available title types (movie, short, TV series, etc.). |

---

## Request and Response Format

**Example Request:**
```http
GET https://moviesdatabase.p.rapidapi.com/titles?year=2023&limit=10&page=1
Headers:
  x-rapidapi-host: moviesdatabase.p.rapidapi.com
  x-rapidapi-key: YOUR_API_KEY
