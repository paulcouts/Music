# Music App 🎵

This is a simple music web application that allows users to search for YouTube videos, view recommended songs, and play them directly within the app using the YouTube IFrame API. The app features an iOS-inspired UI with a hidden video player for seamless music streaming.

---

##  Getting Started

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/music-app.git
cd music-app
```

### 2️⃣ Install Dependencies

Ensure you have Python and pip installed. Then run:

```bash
pip install -r requirements.txt
```

### 3️⃣ Set Up Environment Variables

You **must** copy the `.env.example` file to `.env` and insert your **own YouTube API key** for the project to function properly.

```bash
cp .env.example .env
```

Open the `.env` file and add your YouTube API key:

```env
API_KEY=YOUR_YOUTUBE_API_KEY_HERE
```

>  **Tip:** You can get a YouTube Data API key from the [Google Cloud Console](https://console.cloud.google.com/).

---

##  Running the Application

Start the Flask server by running:

```bash
python app.py
```

The application will be available at:

 [http://localhost:5000](http://localhost:5000)

---

## ⚙️ Features

-  **YouTube Video Playback** — Plays videos using the YouTube IFrame API (audio-focused player).
-  **Search Functionality** — Search for any song or artist and play directly from the search results.
-  **Recommended Songs** — Displays 6 random recommended songs on the home page.
-  **Minimal Player**
-  **Responsive Design** — Optimized for both desktop and mobile devices.

---

##  Troubleshooting

- **Nothing plays when clicking a video:**  
  - Ensure your API key is correct and has YouTube Data API v3 enabled.
  - Check the browser console (`F12`) for any JavaScript or API errors.
  - Some browsers block autoplay by default. Ensure that your browser allows autoplay for media.

- **Search doesn’t return results:**  
  - Verify the `/search` endpoint is working by checking the Flask console logs.
  - Ensure the API key isn't rate-limited.

---

- [YouTube Data API](https://developers.google.com/youtube/v3)  
- [Flask](https://flask.palletsprojects.com/)  
- [YouTube IFrame Player API](https://developers.google.com/youtube/iframe_api_reference)  
```