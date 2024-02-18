# Euterpefy: Music Recommender Application

Welcome to Euterpefy, a project developed by Phuoc Khai Nguyen for a class called CS4750 - Mobile App Development. This project is all about making a music recommendation app that uses Spotify's music data to suggest songs and playlists to users.

## Project Structure

The project has two main parts:

Server-side (Rust API): This part talks to Spotify to get music data, processes this data, and keeps some of it ready so the app can quickly suggest music without having to ask Spotify every time.
Mobile-app (Flutter & Dart): This is the app that you use on your phone. It can directly ask Spotify for some information using the user's Spotify account to make sure the music suggestions are personalized.

## How It Works

Euterpefy uses a mix of both server and app to work efficiently:

- Server-side: This part does the heavy lifting by getting data from Spotify, keeping it ready, and making sure everything runs fast. Uses Rust for its speed and safety. It deals with Spotify, keeps data ready, and sends info to the app.

- Mobile App: For anything specific to the user, like their playlists or music they like, the app talks directly to Spotify. This makes sure the app always has the latest info and can offer music that's just right for the user. Built with Flutter & Dart for a nice looking and easy-to-use interface. It handles logging into Spotify and shows you your music recommendations.

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

## Contributing

This is a personal project by [me]([github](https://github.com/bluesimp1102), so it's not looking for public contributions right now. But feel free to share your thoughts or suggestions through GitHub.

## License

Euterpefy is licensed under the MIT License. See the LICENSE file in each repository for more details.

## Acknowledgments

- Thanks to the instructor of CS4750: Prof. Yu Sun for his teaching materials and support.
- Gratitude to Spotify for providing the API that powers the app's music recommendations.
