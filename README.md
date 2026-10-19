# YouTube Playlist Duration Calculator

A lightweight, responsive web application that calculates the total watch time of a YouTube playlist and estimates how long it will take to watch at different playback speeds.

Built with HTML, CSS, and JavaScript, this tool runs directly in your browser and requires no installation or build process.

## Features

- **Playlist Duration Calculator:** Calculate the combined duration of videos in a YouTube playlist.
- **Multiple URL Formats:** Supports YouTube playlist links, YouTube Music links, mobile links, watch URLs containing a playlist ID, and raw playlist IDs.
- **Playback Speed Estimates:** Estimate watch time at 1×, 1.25×, 1.5×, and 2× speeds.
- **Flexible Duration Formats:** Display the total duration in HH:MM:SS, hours and minutes, or total minutes.
- **Light and Dark Modes:** Switch between themes for a more comfortable viewing experience.
- **Responsive Design:** Works on desktop computers, tablets, and mobile devices.
- **Unavailable Video Detection:** Identifies playlist entries whose durations cannot be retrieved.
- **API Key Visibility Toggle:** Show or hide your YouTube Data API key while entering it.
- **Copy Results:** Copy the calculated results for later reference.
- **Single-File Application:** No package installation, build tools, or additional frameworks are required.

## Technology Stack

- HTML5
- CSS3
- Vanilla JavaScript
- YouTube Data API v3

## Requirements

Before using the calculator, you need:

- A modern web browser.
- An internet connection.
- A Google Cloud project with YouTube Data API v3 enabled.
- A valid YouTube Data API key.
- A public or unlisted YouTube playlist.

## Getting Started

### 1. Download the Project

Clone the repository:

    git clone YOUR_REPOSITORY_URL

Alternatively, download the repository as a ZIP file from GitHub and extract it.

### 2. Open the Application

Open the HTML file in a modern web browser.

For GitHub Pages deployment, rename the main HTML file to `index.html` and place it in the root directory of the repository.

### 3. Configure the YouTube Data API

The calculator uses YouTube Data API v3 to retrieve playlist information and video durations.

To obtain an API key:

1. Visit the [Google Cloud Console](https://console.cloud.google.com/).
2. Create a new project or select an existing project.
3. Open the API Library.
4. Enable **YouTube Data API v3**.
5. Navigate to APIs & Services and open Credentials.
6. Create an API key.
7. Restrict the key to YouTube Data API v3 and configure appropriate application restrictions.

Keep your API key private and never commit it directly to the repository.

### 4. Calculate a Playlist's Duration

1. Open the calculator.
2. Paste a YouTube playlist URL or playlist ID.
3. Enter your YouTube Data API key.
4. Select your preferred duration format.
5. Choose whether to display playback speed estimates.
6. Click the calculate button.
7. Review the total duration and estimated watch times.

## GitHub Pages Deployment

You can host the application using GitHub Pages.

1. Upload the application HTML file to the repository.
2. Rename it to `index.html`.
3. Open your repository's **Settings**.
4. Select **Pages**.
5. Choose deployment from a branch.
6. Select your branch, usually `main`, and the root directory.
7. Save the configuration.

GitHub Pages will provide a website URL when deployment is available.

**Security:** Because the calculator uses a browser-side API key, restrict the key to your website's permitted HTTP referrers and the required API. Do not assume that a browser-side key can remain secret.

## Limitations

- YouTube API requests are subject to Google's quota limits and API policies.
- Private, deleted, restricted, or unavailable videos may not return readable durations.
- The reported total includes only videos whose durations can be retrieved.
- Playback estimates do not account for advertisements, buffering, pauses, or other interruptions.
- API access depends on the validity and configuration of the supplied API key.

## Privacy and Security

The calculator's intended functionality accepts the API key in the browser and uses it for requests to Google's YouTube Data API. Never hard-code a real API key into the source code or publish it in repository files.

Review the HTML source before deployment and use only a cleaned, verified version of the application.

## License and Copyright

**Copyright © 2026. All Rights Reserved.**

This project is proprietary software. No open-source license is granted.

Except for the limited rights necessary to use GitHub's services under its Terms of Service, no permission is granted to use, reproduce, modify, redistribute, commercially exploit, rebrand, or promote this project without prior written permission from the copyright holder.

Unauthorized commercial use, redistribution outside the rights permitted by GitHub, republishing, or use of this project's code, design, or materials for promotional purposes is prohibited to the extent permitted by applicable law.

All rights not expressly granted are reserved by the copyright holder.

Public availability of this repository does not constitute a general license to use, modify, or commercially exploit this project.

## Disclaimer

This project is an independent utility and is not affiliated with, endorsed by, or officially associated with YouTube or Google. YouTube is a trademark of Google LLC.

Use of the YouTube Data API is subject to Google's applicable terms and policies.
