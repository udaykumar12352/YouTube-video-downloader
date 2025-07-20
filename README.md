# YouTube Video Downloader
[![Ask DeepWiki](https://devin.ai/assets/askdeepwiki.png)](https://deepwiki.com/udaykumar12352/YouTube-video-downloader)

This project is a simple web-based application for downloading YouTube videos. It features a clean user interface built with HTML/CSS/JavaScript and a backend powered by Python's FastAPI framework and the `yt-dlp` library.

## Features
*   **Easy to Use:** Simply paste a YouTube video URL and click "Download".
*   **High-Quality Downloads:** Automatically fetches and saves the best available video quality.
*   **Responsive UI:** A clean interface with both light and dark modes available.
*   **Lightweight Backend:** Built with FastAPI for efficient and fast request handling.
*   **Local Downloads:** Videos are saved directly to the directory where the backend server is running.

## Technology Stack
*   **Frontend:** HTML, CSS, JavaScript
*   **Backend:** Python, FastAPI
*   **Video Processing:** `yt-dlp`

## Getting Started

Follow these instructions to get a local copy up and running on your machine.

### Prerequisites
You need to have Python 3 and `pip` installed on your system.

### Installation

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/udaykumar12352/youtube-video-downloader.git
    cd youtube-video-downloader
    ```

2.  **Install the required Python packages:**
    ```sh
    pip install fastapi "uvicorn[standard]" yt-dlp
    ```

### Usage

1.  **Run the Backend Server:**
    Navigate to the project directory in your terminal and run the following command to start the FastAPI server:
    ```sh
    uvicorn backend:app --reload
    ```
    The server will start on `http://localhost:8000`.

2.  **Open the Frontend:**
    Open the `FrontEnd.html` file in your web browser.

3.  **Download a Video:**
    *   Copy a YouTube video URL.
    *   Paste the URL into the input field on the web page.
    *   Click the **Download** button.
    *   The video will be downloaded to the root of the project directory with the filename `Video-{last_11_chars_of_link}.mp4`. A success message will appear on the page to confirm the download has started.
