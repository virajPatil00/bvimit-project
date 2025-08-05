# Campus Connect

A mobile-based centralized event aggregator for college communities built with Flutter.

## 📱 About

Campus Connect is a comprehensive mobile application designed to solve the problem of fragmented event communication in academic institutions. It serves as a unified platform where students, organizers, and administrators can discover, create, and manage campus events efficiently.

## ✨ Features

### For Students
- **Event Discovery**: Browse and search for events across departments and categories
- **Personalized Recommendations**: Get event suggestions based on interests and department
- **Event Registration**: Easy one-tap registration for events
- **Bookmarking**: Save events for later viewing
- **Push Notifications**: Receive timely reminders and updates about registered events
- **QR Code Check-in**: Quick event attendance tracking

### For Event Organizers
- **Event Creation**: Create detailed events with rich information
- **Participant Management**: Track registrations and attendance
- **Real-time Updates**: Send notifications to registered participants
- **Analytics Dashboard**: View event engagement and participation metrics
- **QR Code Generation**: Generate unique QR codes for event check-ins

### For Administrators
- **Event Moderation**: Approve and manage events across the platform
- **User Management**: Manage user roles and permissions
- **Featured Events**: Promote important events on the homepage
- **System Analytics**: View platform-wide usage statistics

## 🛠 Tech Stack

- **Framework**: Flutter 3.10+
- **State Management**: Provider
- **Backend**: Firebase (Authentication, Firestore, Cloud Messaging)
- **Navigation**: Go Router
- **UI Components**: Material Design 3
- **Additional Services**: 
  - Google Sign-In
  - Push Notifications
  - QR Code Generation/Scanning
  - Image Handling

## 📁 Project Structure

```
lib/
├── core/
│   ├── constants/         # App constants and configurations
│   ├── routes/           # Navigation and routing
│   └── theme/            # App theme and styling
├── models/               # Data models
├── providers/            # State management (Provider pattern)
├── services/             # API and business logic services
├── screens/              # UI screens and pages
│   ├── auth/            # Authentication screens
│   ├── events/          # Event-related screens
│   ├── home/            # Home screen
│   ├── main/            # Main wrapper and navigation
│   ├── notifications/   # Notifications screen
│   ├── profile/         # Profile screens
│   ├── search/          # Search functionality
│   └── splash/          # Splash screen
└── widgets/              # Reusable UI components
```

## 🚀 Getting Started

### Prerequisites
- Flutter SDK (3.10 or higher)
- Dart SDK (3.0 or higher)
- Android Studio / VS Code
- Firebase project setup

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/campus-connect.git
   cd campus-connect
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Firebase Setup**
   - Create a new Firebase project
   - Enable Authentication, Firestore, and Cloud Messaging
   - Download `google-services.json` (Android) and `GoogleService-Info.plist` (iOS)
   - Place them in the appropriate directories

4. **Run the app**
   ```bash
   flutter run
   ```

## 🔧 Configuration

### Firebase Configuration
Update the Firebase configuration in `/lib/core/constants/app_constants.dart`:

```dart
static const String firebaseProjectId = 'your-project-id';
```

### API Configuration
Configure your API endpoints:

```dart
static const String baseUrl = 'https://your-api-endpoint.com/v1';
static const String apiKey = 'your-api-key';
```

## 📱 Screens Overview

### Authentication Flow
- **Splash Screen**: App initialization and route determination
- **Login Screen**: Email/password and Google sign-in
- **Register Screen**: User registration with department selection
- **Forgot Password**: Password reset functionality

### Main Application
- **Home Screen**: Dashboard with featured events and quick stats
- **Events Screen**: Complete event listing with filters
- **Search Screen**: Event and user search functionality
- **Profile Screen**: User profile and settings management

### Event Management
- **Event Detail**: Comprehensive event information and registration
- **Create Event**: Event creation form for organizers
- **Event Analytics**: Participation tracking and insights

## 🎨 Design System

The app follows Material Design 3 principles with a custom green color scheme:

- **Primary Color**: `#2E7D32` (Green 800)
- **Secondary Color**: `#4CAF50` (Green 500)
- **Accent Color**: `#81C784` (Green 300)
- **Typography**: Inter font family
- **Component Library**: Custom reusable widgets

## 🔐 Authentication & Security

- Firebase Authentication integration
- Google Sign-In support
- Role-based access control (Student, Organizer, Admin)
- Secure data validation and sanitization
- Privacy-focused user data handling

## 📊 State Management

The app uses the Provider pattern for state management:

- **AuthProvider**: User authentication state
- **EventProvider**: Event data and operations
- **UserProvider**: User profile and notifications

## 🔔 Push Notifications

Firebase Cloud Messaging integration for:
- Event reminders (1 hour before start)
- Event updates and changes
- Registration confirmations
- General announcements

## 🎯 Future Enhancements

- [ ] Event calendar integration
- [ ] Social features (comments, ratings)
- [ ] Event categories and tags
- [ ] Advanced analytics dashboard
- [ ] Offline support and data synchronization
- [ ] Multi-language support
- [ ] Dark mode theme
- [ ] Event sharing and invitations
- [ ] Integration with college management systems

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Support

For support and questions:
- Create an issue on GitHub
- Email: support@campusconnect.com
- Documentation: [docs.campusconnect.com](https://docs.campusconnect.com)

## 🙏 Acknowledgments

- Flutter team for the amazing framework
- Firebase for backend services
- Material Design team for design guidelines
- Open source community for various packages used

---

**Campus Connect** - Connecting campus communities, one event at a time! 🎓✨