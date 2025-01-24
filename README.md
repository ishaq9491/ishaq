<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Movie Explorer</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #fafafa;
    }
    header {
      background-color: #4CAF50;
      color: white;
      padding: 15px;
      text-align: center;
    }
    header h1 {
      margin: 0;
    }
    #search-bar {
      text-align: center;
      margin: 20px 0;
    }
    #search-bar input {
      width: 60%;
      padding: 10px;
      font-size: 16px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    .movie-section {
      padding: 20px;
      color: white;
    }
    .movie-section h2 {
      text-align: center;
      margin-bottom: 20px;
    }
    .action {
      background-color: #ff5722;
    }
    .comedy {
      background-color: #ffeb3b;
      color: black;
    }
    .sci-fi {
      background-color: #2196f3;
    }
    #movie-list {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
    }
    .movie-card {
      background: white;
      border: 1px solid #ddd;
      border-radius: 5px;
      width: 200px;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .movie-card:hover {
      transform: scale(1.1);
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
    }
    .movie-card img {
      width: 100%;
      border-bottom: 1px solid #ddd;
    }
    .movie-card h3 {
      margin: 10px 0;
      font-size: 18px;
    }
    .movie-card p {
      color: #555;
      font-size: 14px;
      margin: 0 10px 10px;
    }
    .movie-card a {
      display: inline-block;
      margin: 5px;
      padding: 10px 15px;
      font-size: 14px;
      text-decoration: none;
      color: white;
      border-radius: 5px;
      transition: background-color 0.3s ease;
    }
    .movie-card a.trailer {
      background-color: #007bff;
    }
    .movie-card a.trailer:hover {
      background-color: #0056b3;
    }
    .movie-card a.tickets {
      background-color: #28a745;
    }
    .movie-card a.tickets:hover {
      background-color: #1e7e34;
    }
  </style>
</head>
<body>
  <header>
    <h1>Movie Explorer</h1>
  </header>
  <div id="search-bar">
    <input type="text" id="search-input" placeholder="Search for a movie..." oninput="filterMovies()">
  </div>

  <!-- Action Movies Section -->
  <div class="movie-section action">
    <h2>Action Movies</h2>
    <div id="movie-list">
      <div class="movie-card" data-title="Mad Max: Fury Road">
        <img src="https://via.placeholder.com/200x300" alt="Mad Max">
        <h3>Mad Max: Fury Road</h3>
        <p>An exhilarating post-apocalyptic adventure.</p>
        <a href="https://www.youtube.com/watch?v=hEJnMQG9ev8" target="_blank" class="trailer">Watch Trailer</a>
        <a href="https://in.bookmyshow.com" target="_blank" class="tickets">Buy Tickets</a>
      </div>
      <div class="movie-card" data-title="John Wick">
        <img src="https://via.placeholder.com/200x300" alt="John Wick">
        <h3>John Wick</h3>
        <p>A relentless tale of revenge.</p>
        <a href="https://www.youtube.com/watch?v=2AUmvWm5ZDQ" target="_blank" class="trailer">Watch Trailer</a>
        <a href="https://in.bookmyshow.com" target="_blank" class="tickets">Buy Tickets</a>
      </div>
    </div>
  </div>

  <!-- Comedy Movies Section -->
  <div class="movie-section comedy">
    <h2>Comedy Movies</h2>
    <div id="movie-list">
      <div class="movie-card" data-title="The Hangover">
        <img src="https://via.placeholder.com/200x300" alt="The Hangover">
        <h3>The Hangover</h3>
        <p>Three friends and one
