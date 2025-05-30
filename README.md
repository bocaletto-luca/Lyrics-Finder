# Lyrics-Finder | API Free | WebAPP
#### Author: Bocaletto Luca

[![HTML5](https://img.shields.io/badge/HTML5-E34F26.svg?style=flat)](https://developer.mozilla.org/en-US/docs/Web/HTML)  
[![CSS3](https://img.shields.io/badge/CSS3-1572B6.svg?style=flat)](https://developer.mozilla.org/en-US/docs/Web/CSS)  
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E.svg?style=flat)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)  
[![Bootstrap 5](https://img.shields.io/badge/Bootstrap-7952B3.svg?style=flat)](https://getbootstrap.com/)  
[![License: GPL](https://img.shields.io/badge/License-GPL-blue.svg)](LICENSE)

## Overview

**Lyrics-Finder** is a free and open-source web application that enables users to explore and retrieve song lyrics through two distinct modes:
- **Direct Search:** Enter an artist’s name and song title to instantly fetch lyrics.
- **Alphabetical Artist Explorer:** Browse artists alphabetically (via a letter menu). For a chosen letter, a paginated list of artists is dynamically retrieved from MusicBrainz. Selecting an artist displays their recordings (with duplicate titles removed and paginated if necessary), and clicking a song fetches its lyrics using the lyrics.ovh API.

This rich, dual-mode interface harnesses the power of MusicBrainz (for dynamic artist and recording data) and lyrics.ovh (for song lyrics) to offer a complete 360° exploration of this open-source music database.

## Features

- **Dual Search Modes:**  
  - **Direct Search:** Users can input both an artist name and a song title to directly retrieve lyrics.
  - **Alphabetical Artist Explorer:** Users pick a letter from an alphabet menu to load a paginated list of artists whose names start with that letter.
- **Dynamic Data Fetching:**  
  - Uses MusicBrainz API (accessed via a free CORS proxy) to dynamically fetch and sort artist and recording data.
  - Queries the lyrics.ovh API to fetch song lyrics.
- **Deduplication & Pagination:**  
  - Removes duplicate song titles (case-insensitive) for cleaner results.
  - Implements pagination for both the artist list (20 per page) and the song list (20 per page) when necessary.
- **Robust Error Handling:**  
  - Informative error messages are displayed if no results are found or if there is an issue during data retrieval.
- **Responsive Design:**  
  - Built with HTML5, CSS3, JavaScript, and Bootstrap 5 to ensure an optimal experience across devices.

## Usage

1. **Direct Search:**  
   On the main landing area, users can manually enter an artist name and song title to instantly fetch lyrics.

2. **Alphabetical Artist Explorer:**  
   At the top of the page, an alphabet menu (A–Z) allows users to choose a letter. When a letter is clicked:
   - The app queries MusicBrainz for artists whose names start with that letter.
   - The artist list is paginated (20 artists per page) and displayed in a grid.
   - Clicking on an artist card brings up the artist's available recordings (songs). Duplicate song titles are filtered out.
   - If the artist has many songs, the list is paginated.
   - Clicking on a song fetches its lyrics via the lyrics.ovh API and shows them in a fullscreen modal.

## Technologies Used

- **HTML5** – Provides the structured, semantic markup.
- **CSS3** – Used for styling and responsive layouts.
- **JavaScript** – Implements dynamic functionality and API integrations.
- **Bootstrap 5** – Ensures a modern, responsive design.
- **MusicBrainz API** – Dynamically retrieves artist and recording data (accessed via a free CORS proxy).
- **lyrics.ovh API** – Fetches song lyrics based on artist and title.

## Contributing

Contributions are welcome! Please fork the repository, open issues for any bugs or feature requests, and submit pull requests to help enhance this open-source project.

## License

This project is licensed under the **GPL License**. See the [LICENSE](LICENSE) file for more details.

## About the Author

**Bocaletto Luca**  
GitHub: [bocaletto-luca](https://github.com/bocaletto-luca)

Lyrics-Finder is developed by Bocaletto Luca, a passionate advocate for creating 100% free, open source, and open data web applications.

---

Enjoy exploring and finding your favorite song lyrics – oh yeah friend!
