# CineSeek API Integration

## API Overview
The MoviesDatabase API provides access to a large collection of movie data, including titles, genres, release years, cast, and crew information. It supports filtering, pagination, and searching by multiple parameters, making it suitable for movie discovery applications.

## Version
v1 (from the MoviesDatabase API documentation)

## Available Endpoints
- **/titles** – Fetch a list of movies. Supports filters such as year and genre, with pagination support.
- **/titles/{id}** – Retrieve detailed information for a specific movie by ID.
- **/genres** – Get the list of available genres for filtering.
- **/people** – Access information about actors, directors, and other crew members.
- **/search** – Search for movies or people by name or keyword.

## Request and Response Format
**Example Request:**
```http
GET /titles?year=2023&genre=action&page=1
Host: moviesdatabase.p.rapidapi.com
Headers:
  X-RapidAPI-Key: YOUR_API_KEY
  X-RapidAPI-Host: moviesdatabase.p.rapidapi.com
