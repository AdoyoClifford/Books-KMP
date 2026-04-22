<div align="center">

# 📚 Books KMP

**A Kotlin Multiplatform book discovery app for Android, iOS & Desktop**

[![Kotlin](https://img.shields.io/badge/Kotlin-92.1%25-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org/)
[![Compose Multiplatform](https://img.shields.io/badge/Compose%20Multiplatform-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white)](https://www.jetbrains.com/lp/compose-multiplatform/)
[![Swift](https://img.shields.io/badge/Swift-7.9%25-F05138?style=for-the-badge&logo=swift&logoColor=white)](https://developer.apple.com/swift/)

</div>

---

## 📖 About

Books KMP is a **Kotlin Multiplatform** application that demonstrates sharing business logic and UI across Android, iOS, and Desktop platforms using **Compose Multiplatform**. It showcases modern KMP development practices with a clean architecture approach.

## 🎯 Platforms Supported

| Platform | Status | UI Framework |
|---|---|---|
| 🤖 **Android** | ✅ Supported | Compose Multiplatform |
| 🍎 **iOS** | ✅ Supported | Compose Multiplatform + SwiftUI entry point |
| 🖥️ **Desktop** | ✅ Supported | Compose Multiplatform |

## 🏗️ Architecture

```
┌─────────────────────────────────────────┐
│              Shared Code                │
│  ┌───────────────────────────────────┐  │
│  │         commonMain               │  │
│  │  ┌─────────┐  ┌──────────────┐   │  │
│  │  │  Domain  │  │  Presentation│   │  │
│  │  └─────────┘  └──────────────┘   │  │
│  │  ┌─────────┐  ┌──────────────┐   │  │
│  │  │  Data   │  │  Shared UI   │   │  │
│  │  └─────────┘  └──────────────┘   │  │
│  └───────────────────────────────────┘  │
├──────────┬──────────┬───────────────────┤
│ Android  │   iOS    │     Desktop       │
│  Main    │  Main    │      Main         │
└──────────┴──────────┴───────────────────┘
```

## 🛠️ Tech Stack

| Category | Technology |
|---|---|
| **Language** | Kotlin, Swift (iOS entry point) |
| **Shared UI** | Compose Multiplatform |
| **Architecture** | Clean Architecture |
| **Build System** | Gradle (Kotlin DSL) |
| **Multiplatform** | Kotlin Multiplatform (KMP) |

## 🚀 Getting Started

### Prerequisites

- **Android Studio** (Ladybug or later) with KMP plugin
- **JDK 17+**
- **Xcode 15+** (for iOS development)

### Running the App

#### Android
```bash
# Open in Android Studio and run the androidApp configuration
./gradlew :composeApp:assembleDebug
```

#### iOS
```bash
# Open iosApp/iosApp.xcodeproj in Xcode and run
```

#### Desktop
```bash
./gradlew :composeApp:run
```

## 📁 Project Structure

```
Books-KMP/
├── composeApp/                # Shared Compose Multiplatform code
│   └── src/
│       ├── commonMain/        # Shared code for all platforms
│       ├── androidMain/       # Android-specific implementations
│       ├── iosMain/           # iOS-specific implementations
│       └── desktopMain/       # Desktop-specific implementations
├── iosApp/                    # iOS app entry point (SwiftUI)
├── build.gradle.kts           # Root build configuration
├── gradle.properties
└── settings.gradle.kts
```

## 📚 Learn More

- [Kotlin Multiplatform Documentation](https://www.jetbrains.com/help/kotlin-multiplatform-dev/get-started.html)
- [Compose Multiplatform](https://www.jetbrains.com/lp/compose-multiplatform/)
- [KMP Samples](https://www.jetbrains.com/help/kotlin-multiplatform-dev/multiplatform-samples.html)

## 🤝 Contributing

Contributions are welcome! Feel free to open issues or submit PRs.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---


