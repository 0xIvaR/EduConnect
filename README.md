# 🎓 EduConnect

<div align="center">
  <h3>A Modern Android Learning Management Application</h3>
  <p>Connecting students and teachers through intuitive design and powerful functionality</p>
  
  <img src="https://img.shields.io/badge/Platform-Android-brightgreen" alt="Platform">
  <img src="https://img.shields.io/badge/Language-Kotlin-blue" alt="Language">
  <img src="https://img.shields.io/badge/Firebase-Integrated-orange" alt="Firebase">
  <img src="https://img.shields.io/badge/License-MIT-yellow" alt="License">
</div>

---

## 📱 About EduConnect

EduConnect is a comprehensive Android learning management application designed to bridge the gap between students and educators. Built with modern Android development practices, it provides a seamless experience for both learners and instructors with role-based authentication and personalized dashboards.

## ✨ Key Features

### 🔐 Authentication & Security
- **Dual Login System**: Separate authentication flows for students and teachers
- **Firebase Authentication**: Secure email/password authentication
- **Role-Based Access**: Different interfaces based on user type
- **Session Management**: Secure logout with session cleanup

### 👥 User Experience
- **Welcome Screen**: Intuitive app introduction and navigation
- **Personalized Dashboards**: Customized home screens for each user type
- **Theme Support**: Dynamic dark/light theme switching
- **Responsive UI**: Material Design principles throughout

### 🏗️ Technical Architecture
- **Firebase Firestore**: Real-time database for user profiles and data
- **MVVM Pattern**: Clean architecture with proper separation of concerns
- **Kotlin Coroutines**: Asynchronous programming for smooth performance
- **Material Design**: Modern, accessible UI components

## 🛠️ Technology Stack

- **Language**: Kotlin
- **Platform**: Android (API 21+)
- **Architecture**: MVVM + Repository Pattern
- **Database**: Firebase Firestore
- **Authentication**: Firebase Auth
- **UI Framework**: Material Design Components
- **Async Operations**: Kotlin Coroutines & Flow
- **Build System**: Gradle with Kotlin DSL

## 🚀 Getting Started

### Prerequisites

Before you begin, ensure you have the following installed:
- **Android Studio**: Arctic Fox (2021.3.1) or newer
- **Java/Kotlin**: JDK 11 or higher
- **Android SDK**: API level 21 or higher
- **Firebase Account**: For backend services

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/educonnect.git
   cd educonnect
   ```

2. **Firebase Setup**
   - Visit [Firebase Console](https://console.firebase.google.com/)
   - Create a new project or use existing one
   - Add Android app with package name: `com.example.educonnect`
   - Download `google-services.json` and place in `app/` directory

3. **Configure Firebase Services**
   ```bash
   # Enable Authentication
   # Go to Authentication > Sign-in method > Enable Email/Password
   
   # Setup Firestore Database
   # Go to Firestore Database > Create database > Production mode
   ```

4. **Build and Run**
   ```bash
   # Open in Android Studio
   # Sync Gradle files
   # Build and run on device/emulator
   ```

## 📊 Database Schema

### Firestore Structure
```
/users/{userId}
├── email: string
├── userType: "student" | "teacher"
├── name: string
├── uniqueId: string (teachers only)
├── grade: string (students only)
├── subject: string (teachers only)
└── createdAt: timestamp
```

## 🔑 Demo Credentials

For testing purposes, you can use these pre-configured accounts:

| User Type | Identifier | Password |
|-----------|------------|----------|
| Student | `student@example.com` | `password123` |
| Teacher | `teacher001` | `password123` |

### Quick Setup Method
1. Run the application in Android Studio
2. Long press the app logo on the welcome screen
3. Demo accounts will be automatically created

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Development Commands

```bash
# Build the project
./gradlew build

# Install debug version
./gradlew installDebug

# Run unit tests
./gradlew test

# Run instrumented tests
./gradlew connectedAndroidTest

# Generate APK
./gradlew assembleDebug
```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Material Design Components](https://material.io/components) for beautiful UI elements
- [Firebase](https://firebase.google.com/) for robust backend services
- [Kotlin Coroutines](https://kotlinlang.org/docs/coroutines-overview.html) for asynchronous programming
- [Android Jetpack](https://developer.android.com/jetpack) for modern Android development

---

<div align="center">
  <p>Made with ❤️ for education</p>
  <p>If you found this project helpful, please consider giving it a ⭐</p>
</div> 