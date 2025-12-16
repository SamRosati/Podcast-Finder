# Podcast Finder

<div align="center">
  <h3>A Web Interface for Discovering Podcasts</h3>
  <p>Created by Sam Rosati</p>
</div>

## About The Project

**Podcast Finder** is a web-based application that allows users to search for podcasts, episodes, and curated lists.

The primary objective of this project was to solidify my understanding of **HTML** and **CSS**, specifically focusing on how to structure complex forms and handle data transmission. It serves as a practical exercise in understanding the difference between HTTP `GET` and `POST` requests by integrating a real-world API into a standard HTML form.

## Key Features

* **Live Podcast Search:** Integrated directly with the **ListenNotes API** to perform real-time searches.
* **Advanced Filtering:** Users can refine search results by:
    * Type (Episode, Podcast, Curated).
    * Minimum / Maximum duration.
    * Language.
    * Publish Date.
* **Responsive Design:** A mobile-friendly layout that utilizes **CSS Grid** to adapt from a stacked mobile view to a two-column desktop interface (min-width: 900px).
* **Contact Interface:** A demonstration of a user feedback form including text inputs, dropdowns for age selection, and checkboxes for category interests.
* **Interactive UI:** Custom styling for hover and active states on buttons and inputs to improve user experience.

## Tech Stack

* **HTML5:** Semantic structure for forms, inputs, and layout.
* **CSS3:** Custom styling using CSS Grid, Flexbox, and Media Queries.
* **API:** [ListenNotes API](https://www.listennotes.com/api/) (via Form Action).
* **Fonts:** **Mukta** and **Saira Condensed** from Google Fonts.

## Learning Outcomes

This project focused on the core fundamentals of web forms and data handling:

1.  **GET Requests:** Implemented in the "Find a Podcast" form.
    * The form sends data to `https://www.listennotes.com/search`.
    * Input `name` attributes (like `q`, `len_min`, `type`) correspond to the API's query parameters, allowing the URL to carry the search data.

2.  **POST Requests:** Implemented in the "Contact Us" form.
    * Demonstrates how sensitive data (like user feedback) is structured for submission in the request body rather than the URL.

3.  **CSS Grid Layouts:**
    * Used `display: grid` to create a structured layout for labels and inputs.
    * Implemented media queries to shift input fields into a second column on larger screens (`grid-column: 2/3`) while keeping labels aligned to the left.

## How to Use

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/SamRosati/Podcast-Finder.git](https://github.com/SamRosati/Podcast-Finder.git)
    ```
2.  **Open the Project:**
    Open `index.html` in your web browser.
3.  **Search:**
    Enter a keyword (e.g., "Tech"), select filters, and click "Search". You will be redirected to ListenNotes with your specific search criteria applied.
