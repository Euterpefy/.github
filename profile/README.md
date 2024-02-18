# Euterpefy: Music Recommender Application

Welcome to the Euterpefy GitHub organization! This project, developed as a coursework assignment for CS4750 - Mobile App Development, is a hybrid music recommender system designed to enhance user experience by providing personalized music recommendations. Utilizing both a server-side API and direct client-side requests to the Spotify API, Euterpefy offers a unique approach to music discovery by leveraging cached data for efficiency and user-specific data for personalization.

## Project Structure

Euterpefy is divided into two main components:

- **server-side**: A Rust-based API that serves as the intermediary between the mobile app and the Spotify API. It's responsible for fetching, processing, and caching data from Spotify to optimize API call efficiency and provide quick responses to the mobile app.
- **mobile-app**: A mobile application developed with Flutter & Dart, providing a user-friendly interface for accessing music recommendations. It directly interacts with the Spotify API using the logged-in user's token for operations that require real-time data or user-specific information.

## How It Works

Euterpefy employs a hybrid model to deliver music recommendations:

1. **Server-side Caching**: To reduce the number of API calls and enhance response times, the server-side component caches essential data from Spotify. This includes popular tracks, genres, and artist information that can be used to generate recommendations for multiple users.

2. **Client-side Requests**: For user-specific queries, such as fetching a user's playlists or liked songs, the mobile app directly communicates with the Spotify API using the user's personal access token. This approach ensures that recommendations are personalized and up-to-date.

### Server-side (Rust API)

The server-side API is built with Rust, offering high performance and reliability. It handles:
- Communication with the Spotify API to fetch and process data.
- Caching of frequently accessed data to improve efficiency.
- Serving processed data to the mobile app to generate recommendations.

### Mobile App (Flutter & Dart)

The mobile application is where users interact with Euterpefy. It features:
- Authentication with Spotify to access user-specific data.
- Direct requests to the Spotify API for real-time, personalized content.
- A sleek and responsive UI for browsing music recommendations.

## Getting Started

To explore Euterpefy, clone the respective repositories for the server-side API and mobile app. Detailed setup instructions are available in each repository's README.md.

### Prerequisites

- Rust environment and Cargo for the server-side API.
- Flutter SDK and Dart for the mobile application.
- An IDE or editor that supports Flutter and Dart (e.g., Visual Studio Code, Android Studio).

## Contributing

Given that Euterpefy is a coursework project, contributions are limited to project team members. However, we welcome feedback and suggestions through GitHub issues.

## License

Euterpefy is licensed under the MIT License. See the LICENSE file in each repository for more details.

## Acknowledgments

- Thanks to the instructor of CS4750: Prof. Yu Sun for his teaching materials and support.
- Gratitude to Spotify for providing the API that powers the app's music recommendations.
