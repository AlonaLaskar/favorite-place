# Favorite Places App

## Overview
Great Places is a Flutter application that allows users to save their favorite places, including images and locations, and view them later. It utilizes Firebase for authentication and Firestore for data storage.

## Features
- Add new places with an image and location
- Store places persistently
- View a list of saved places
- View place details with a map
- Capture or select images
- Use Google Maps API for location selection
- Supports Riverpod for state management

## Technologies Used
- **Flutter**: Cross-platform framework
- **Firebase Firestore**: Database for storing places
- **Firebase Authentication**: User authentication
- **Google Maps API**: For map-based location selection
- **Image Picker**: Capture or select images
- **Riverpod**: State management

## Installation
### Prerequisites
Ensure you have the following installed:
- Flutter SDK
- Dart
- Firebase CLI
- Google Maps API key

### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/AlonaLaskar/favorite-place.git
   cd great_places
   ```
2. Install dependencies:
   ```sh
   flutter pub get
   ```
3. Configure Firebase:
   - Set up Firebase for your project
   - Run `flutterfire configure` to generate Firebase configuration files
   
4. Configure Google Maps API Key:
   - Add your API key to the `.env` file
   ```
   GOOGLE_API_KEY=your_api_key_here
   ```
   
5. Run the app:
   ```sh
   flutter run
   ```

## Project Structure
```
great_places/
│── lib/
│   │── main.dart              # Entry point of the application
│   │── models/
│   │   │── place.dart         # Place model
│   │── providers/
│   │   │── user_place.dart    # User places provider
│   │── screens/
│   │   │── places.dart        # Main screen for viewing places
│   │   │── add_place.dart     # Add new places
│   │   │── place_detail.dart  # Place detail screen
│   │── widgets/
│   │   │── image_input.dart   # Image picker widget
│   │   │── location_input.dart # Location picker widget
│── pubspec.yaml               # Project dependencies
```

## Usage
- Open the app
- Add a new place by selecting an image and a location
- View and manage saved places

## Dependencies
```yaml
flutter_riverpod: ^2.0.0
firebase_core: ^3.10.0
firebase_auth: ^5.4.0
firebase_storage: ^12.4.0
image_picker: ^1.1.2
cloud_firestore: ^5.6.1
flutter_dotenv: ^5.0.2
location: ^5.0.0
``` 

⭐⭐⭐⭐⭐