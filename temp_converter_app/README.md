# Temperature Converter App

A responsive Flutter application for converting temperatures between Fahrenheit and Celsius with conversion history tracking.

## Features

- **Bidirectional Conversion**: Convert between Fahrenheit to Celsius and Celsius to Fahrenheit
- **Responsive Design**: Optimized for both portrait and landscape orientations
- **Conversion History**: Track and display previous conversions
- **Clean UI**: Purple-themed interface with intuitive controls
- **Cross-Platform**: Works on Android, iOS, Web, and Desktop

## Layouts

The app adapts to different screen sizes and orientations:
- Portrait mode: Vertical layout with stacked components
- Landscape mode: Horizontal layout with input controls on the left and history on the right

## Getting Started

### Prerequisites

- Flutter SDK (latest stable version)
- Dart SDK (included with Flutter)
- Android Studio or VS Code with Flutter extensions
- For Android: Android SDK and emulator
- For iOS: Xcode (macOS only)

### Installation

1. **Clone or download the project**
   ```bash
   git clone <repository-url>
   cd temp_converter_app
   ```


2. **Verify Flutter installation**
   ```bash
   flutter doctor
   ```

### Running the App

#### On Physical Device
1. Enable Developer Options and USB Debugging on your device
2. Connect your device via USB
3. Run the app:
   ```bash
   flutter run
   ```

#### On Android Emulator
1. **Create an Android emulator:**
   ```bash
   flutter emulators
   flutter emulators --launch <emulator-id>
   ```
   Or use Android Studio:
   - Open Android Studio
   - Go to Tools > AVD Manager
   - Create a new Virtual Device
   - Start the emulator

2. **Run the app:**
   ```bash
   flutter run
   ```

#### On iOS Simulator (macOS only)
1. **Open iOS Simulator:**
   ```bash
   open -a Simulator
   ```

2. **Run the app:**
   ```bash
   flutter run
   ```

#### On Web
```bash
flutter run -d chrome
```

#### On Desktop
```bash
# Windows
flutter run -d windows

# macOS
flutter run -d macos

# Linux
flutter run -d linux
```

### Building for Release

#### Android APK
```bash
flutter build apk --release
```

#### Android App Bundle
```bash
flutter build appbundle --release
```

#### iOS
```bash
flutter build ios --release
```

#### Web
```bash
flutter build web --release
```

## How to Use

1. **Select Conversion Type**: Choose between "Fahrenheit to Celsius" or "Celsius to Fahrenheit" using the radio buttons
2. **Enter Temperature**: Input the temperature value in the text field
3. **Convert**: Press the "CONVERT" button to see the result
4. **View History**: Previous conversions are automatically saved and displayed in the history section

## Project Structure

```
lib/
└── main.dart          # Main application file with all UI components and logic
```

## Key Components

- **TempConverterApp**: Main app widget with Material Design theme
- **TempConverterHome**: Stateful widget containing the conversion logic
- **Responsive Layout**: Automatic adaptation between portrait and landscape modes
- **Conversion Logic**: Accurate temperature conversion formulas
- **History Management**: List-based storage of conversion history

## Technical Details

- **Framework**: Flutter
- **Language**: Dart
- **State Management**: StatefulWidget with setState
- **UI Components**: Material Design widgets
- **Responsive Design**: MediaQuery and LayoutBuilder

## Troubleshooting

### Common Issues

1. **Flutter not recognized**: Make sure Flutter is added to your PATH
2. **No devices found**: Ensure emulator is running or device is connected
3. **Build errors**: Run `flutter clean` then `flutter pub get`
4. **Emulator issues**: Try wiping emulator data or creating a new one

### Useful Commands

```bash
# Check Flutter installation
flutter doctor

# List available devices
flutter devices

# Clean project
flutter clean

# Get dependencies
flutter pub get

# Run with hot reload
flutter run

# Build release APK
flutter build apk --release
```

## Contributing

1. Fork the project
2. Create a feature branch
3. Make your changes
4. Test thoroughly on different devices/orientations
5. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).
