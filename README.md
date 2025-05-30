# Lyrics-Finder | API Free | WebAPP
#### Author: Bocaletto Luca

[![HTML5](https://img.shields.io/badge/HTML5-E34F26.svg?style=flat)](https://developer.mozilla.org/en-US/docs/Web/HTML) [![CSS3](https://img.shields.io/badge/CSS3-1572B6.svg?style=flat)](https://developer.mozilla.org/en-US/docs/Web/CSS) [![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E.svg?style=flat)](https://developer.mozilla.org/en-US/docs/Web/JavaScript) [![Bootstrap 5](https://img.shields.io/badge/Bootstrap-7952B3.svg?style=flat)](https://getbootstrap.com/) [![License: GPL](https://img.shields.io/badge/License-GPL-blue.svg)](LICENSE)

## Overview

**Lyrics-Finder** is a free and open-source web application that lets you retrieve song lyrics in two powerful ways:

1. **Direct Search:**  
   Quickly fetch lyrics by entering both an artist's name and a song title.

2. **Alphabetical Artist Explorer:**  
   Browse through an A–Z menu to dynamically query and list artists (using the MusicBrainz API via a free CORS proxy). For a chosen letter, a paginated list of artists (20 per page) is displayed. Select an artist to view their recordings (with duplicate titles removed and, if necessary, paginated), and then click on a song to retrieve its lyrics via the lyrics.ovh API, shown in a fullscreen modal.

This dual-mode interface offers an end-to-end exploration of song lyrics using completely free, open source APIs and technologies.

## Features

- **Dual Search Modes:**  
  - *Direct Search:* Type in both an artist and song title to instantly retrieve lyrics.  
  - *Alphabetical Explorer:* Choose a letter from an alphabet menu to dynamically fetch and display a paginated list of artists, and then their sorted recording list.
  
- **Dynamic Data Integration:**  
  - Leverages the MusicBrainz API (accessed via a free CORS proxy) to fetch and sort artist and recording data based solely on the first letter of artists’ names.
  - Uses the lyrics.ovh API for fetching song lyrics.

- **Deduplication & Pagination:**  
  - Automatically filters out duplicate song titles (case-insensitive) for a cleaner display.
  - Implements pagination for the artist list (20 per page) and the song list (20 per page) when needed.

- **Robust Error Handling:**  
  - Displays informative error messages if no data, duplicate entries, or missing lyrics are encountered.

- **Responsive and Professional Design:**  
  - Built with HTML5, CSS3, JavaScript, and Bootstrap 5 to ensure the interface is modern and adapts to any device.

## Usage

### Direct Search
- On the landing page, simply enter an artist’s name and a song title. Clicking the search button will immediately fetch and display the lyrics in a fullscreen modal.

### Alphabetical Artist Explorer
- **Alphabet Menu:**  
  At the top of the page, an A–Z menu is available.  
  Clicking a letter dynamically fetches artists from MusicBrainz whose names start with that letter.

- **Artist Listing:**  
  The list is displayed in a grid with pagination (20 artists per page).  
  Click on an artist card to view a list of the artist’s recordings.

- **Song Listing:**  
  Recordings (song titles) are deduplicated and sorted alphabetically.  
  If more than 20 songs are found, pagination will be available.

- **Lyrics Modal:**  
  Clicking on a song calls the lyrics.ovh API to retrieve the lyrics, which are then displayed in a fullscreen modal.

## Technologies Used

- **HTML5** – Structured, semantic markup.
- **CSS3** – Styling and layout design.
- **JavaScript** – Dynamic functionality and API integrations.
- **Bootstrap 5** – Responsive design and UI components.
- **MusicBrainz API** – Dynamically retrieves artist and recording data (via a free CORS proxy).
- **lyrics.ovh API** – Fetches song lyrics based on artist and title.

## Contributing

Contributions are welcome! If you spot bugs, have feature suggestions, or want to improve the interface, please fork the repository and submit a pull request. Let’s work together to make this tool even better.

## License

This project is licensed under the **GPL License**. See the [LICENSE](LICENSE) file for further details.

## About the Author

**Bocaletto Luca**  
GitHub: [bocaletto-luca](https://github.com/bocaletto-luca)

Lyrics-Finder is developed by Bocaletto Luca, a passionate advocate for creating 100% free, open source, and open data web applications.

---

Enjoy exploring and discovering your favorite song lyrics – oh yeah friend!
