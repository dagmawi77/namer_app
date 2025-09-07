# Namer App

A Flutter application that generates random word pairs and allows users to save their favorites. This project demonstrates state management using the Provider package and showcases modern Flutter development practices.

## Features

- 🎲 **Random Word Generation**: Generates random word pairs using the `english_words` package
- ❤️ **Favorites System**: Like and save your favorite word combinations
- 🎨 **Modern UI**: Clean, Material Design interface with customizable theming
- 📱 **Cross-Platform**: Runs on Android, iOS, Web, Windows, macOS, and Linux
- 🔄 **State Management**: Uses Provider pattern for efficient state management

## Screenshots

The app features a simple, intuitive interface:
- Large card displaying the current word pair
- Like button to add/remove from favorites
- Next button to generate new word pairs

## Getting Started

### Prerequisites

- Flutter SDK (3.8.1 or higher)
- Dart SDK
- Android Studio / VS Code with Flutter extensions
- Platform-specific development tools (Android SDK, Xcode for iOS, etc.)

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd namer_app
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the app**
   ```bash
   flutter run
   ```

### Platform-Specific Setup

#### Android
- Ensure Android SDK is installed
- Connect an Android device or start an emulator

#### iOS (macOS only)
- Install Xcode
- Run `pod install` in the `ios` directory
- Connect an iOS device or start the simulator

#### Web
```bash
flutter run -d chrome
```

#### Desktop (Windows/macOS/Linux)
```bash
flutter run -d windows  # Windows
flutter run -d macos    # macOS
flutter run -d linux    # Linux
```

## Project Structure

```
lib/
├── main.dart          # Main application entry point
├── models/            # Data models (if any)
├── screens/           # UI screens
├── widgets/           # Reusable widgets
└── providers/         # State management providers
```

## Dependencies

- **flutter**: Flutter SDK
- **english_words**: Random word pair generation
- **provider**: State management and dependency injection

## Development

### Code Style
This project follows Flutter's official style guide and uses `flutter_lints` for code analysis.

### Running Tests
```bash
flutter test
```

### Building for Production

#### Android
```bash
flutter build apk --release
```

#### iOS
```bash
flutter build ios --release
```

#### Web
```bash
flutter build web --release
```

## Architecture

The app uses a simple but effective architecture:

- **Provider Pattern**: For state management and dependency injection
- **Stateless Widgets**: For UI components that don't need to maintain state
- **ChangeNotifier**: For managing app state and notifying listeners of changes

### Key Components

- `MyApp`: Root widget with theme configuration
- `MyAppState`: State management class using ChangeNotifier
- `MyHomePage`: Main screen displaying word pairs and controls
- `BigCard`: Reusable widget for displaying word pairs

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Flutter team for the amazing framework
- The `english_words` package maintainers
- Provider package contributors

## Future Enhancements

- [ ] Add animations and transitions
- [ ] Implement word pair history
- [ ] Add sharing functionality
- [ ] Create custom themes
- [ ] Add word definitions
- [ ] Implement offline storage
- [ ] Add search functionality for favorites

---

**Note**: This is a learning project demonstrating Flutter fundamentals and state management patterns.