# Zero Hunger - Leftover Food Share App

A Flutter mobile application that connects restaurants with local shelters to reduce food waste and help feed those in need. This app addresses the UN Sustainable Development Goal #2: Zero Hunger by facilitating the distribution of leftover food from restaurants to shelters.

## 🎯 Features

### For Restaurants
- **Add Food Donations**: Easily list leftover food with details like type, quantity, and expiry date
- **Track Donations**: Monitor the status of donations (available, claimed, completed)
- **Dashboard**: View donation statistics and history
- **Pickup Instructions**: Provide specific instructions for food pickup

### For Shelters
- **Browse Available Food**: View all available food donations from nearby restaurants
- **Claim Donations**: Reserve food donations for pickup
- **Track Claims**: Monitor claimed donations and mark them as completed
- **Real-time Updates**: Get notified when new donations become available

### General Features
- **User Authentication**: Simple login system for restaurants and shelters
- **Intuitive UI**: Clean, user-friendly interface with Material Design
- **Real-time Data**: Mock real-time updates for donation status
- **Responsive Design**: Works on various screen sizes

## 🚀 Getting Started

### Prerequisites

Before running this app, make sure you have:

- [Flutter SDK](https://flutter.dev/docs/get-started/install) (version 3.22.2 or later)
- [Dart SDK](https://dart.dev/get-dart) (included with Flutter)
- An IDE with Flutter support:
  - [Android Studio](https://developer.android.com/studio) with Flutter plugin
  - [VS Code](https://code.visualstudio.com/) with Flutter extension
  - [IntelliJ IDEA](https://www.jetbrains.com/idea/) with Flutter plugin

### Installation

1. **Clone or download the project**
   ```bash
   # If you have the project as a zip file, extract it
   # If you have git access:
   git clone <repository-url>
   cd zero_hunger_app
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Run the app**
   ```bash
   # For debug mode
   flutter run
   
   # For release mode
   flutter run --release
   ```

### Running on Different Platforms

#### Android
- Connect an Android device via USB with USB debugging enabled, or
- Start an Android emulator from Android Studio

#### iOS (macOS only)
- Connect an iOS device, or
- Start an iOS simulator

#### Web
```bash
flutter run -d chrome
```

#### Desktop (Linux/Windows/macOS)
```bash
# Linux
flutter run -d linux

# Windows
flutter run -d windows

# macOS
flutter run -d macos
```

## 📱 How to Use

### For Restaurants

1. **Login**
   - Open the app
   - Select "Restaurant" as user type
   - Enter any email and password (demo app)
   - Tap "Login"

2. **Add Food Donation**
   - Tap the "Add Donation" floating action button
   - Fill in the food details:
     - Food Type (from dropdown)
     - Description
     - Quantity (number of servings)
     - Expiry Date
     - Pickup Instructions (optional)
   - Tap "Add Donation"

3. **Manage Donations**
   - View all your donations on the dashboard
   - Check donation status (Available, Claimed, Completed, Expired)
   - See which shelter claimed your donation

### For Shelters

1. **Login**
   - Open the app
   - Select "Shelter" as user type
   - Enter any email and password (demo app)
   - Tap "Login"

2. **Browse Available Food**
   - View the "Available Donations" tab
   - See food details, restaurant info, and expiry dates
   - Tap "Claim" to reserve food for pickup

3. **Manage Claims**
   - Switch to "My Claims" tab
   - View all your claimed donations
   - Tap "Complete" when you've picked up the food

## 🏗️ Project Structure

```
lib/
├── main.dart                 # App entry point
├── models/                   # Data models
│   ├── user.dart            # User model (Restaurant/Shelter)
│   └── food_donation.dart   # Food donation model
├── screens/                  # UI screens
│   ├── login_screen.dart    # Login/authentication screen
│   ├── restaurant_dashboard.dart  # Restaurant main screen
│   ├── shelter_dashboard.dart     # Shelter main screen
│   └── add_donation_screen.dart   # Add new donation screen
└── services/                 # Business logic
    ├── auth_service.dart     # Authentication service
    └── donation_service.dart # Donation management service
```

## 🎨 Design Principles

- **Material Design**: Follows Google's Material Design guidelines
- **Accessibility**: Designed with accessibility in mind
- **Responsive**: Adapts to different screen sizes
- **Intuitive**: Simple and easy-to-use interface
- **Consistent**: Uniform design language throughout the app

## 🔧 Technical Details

### Architecture
- **Pattern**: Simple MVC-like architecture
- **State Management**: Built-in Flutter state management (setState)
- **Data Storage**: In-memory mock data (for demo purposes)
- **Navigation**: Flutter's built-in navigation

### Key Dependencies
- `flutter/material.dart` - Material Design components
- `flutter/cupertino.dart` - iOS-style components (if needed)

### Mock Data
The app uses mock data for demonstration purposes:
- Sample restaurants and shelters
- Pre-populated food donations
- Simulated API delays for realistic experience

## 🚧 Future Enhancements

### Planned Features
- **Real Backend Integration**: Connect to actual API
- **Push Notifications**: Real-time notifications for new donations
- **Location Services**: GPS-based matching of nearby restaurants and shelters
- **Photo Upload**: Add photos of food donations
- **Rating System**: Rate restaurants and shelters
- **Analytics**: Detailed analytics for food waste reduction
- **Multi-language Support**: Support for multiple languages

### Technical Improvements
- **State Management**: Implement Provider or Bloc pattern
- **Database**: Add local database (SQLite) for offline support
- **API Integration**: RESTful API integration
- **Testing**: Comprehensive unit and integration tests
- **CI/CD**: Automated testing and deployment

## 🤝 Contributing

This is a demo application created for educational purposes. To contribute:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📄 License

This project is created for educational and demonstration purposes. Feel free to use it as a starting point for your own projects.

## 🆘 Troubleshooting

### Common Issues

1. **Flutter not found**
   - Make sure Flutter is installed and added to your PATH
   - Run `flutter doctor` to check your setup

2. **Dependencies not found**
   - Run `flutter pub get` to install dependencies
   - Try `flutter clean` followed by `flutter pub get`

3. **Build errors**
   - Make sure you're using a compatible Flutter version
   - Check that all required SDKs are installed

4. **App not running**
   - Ensure you have a connected device or emulator
   - Check that USB debugging is enabled (Android)

### Getting Help

- Check the [Flutter documentation](https://flutter.dev/docs)
- Visit [Flutter community](https://flutter.dev/community)
- Search [Stack Overflow](https://stackoverflow.com/questions/tagged/flutter)

## 🌟 Acknowledgments

- Flutter team for the amazing framework
- Material Design team for the design system
- UN Sustainable Development Goals for inspiration
- Open source community for tools and resources

---

**Note**: This is a demonstration app with mock data. In a production environment, you would need to implement proper backend services, authentication, and data persistence.

