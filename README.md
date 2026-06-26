<div align="center">
  <img src="app_logo.png" alt="Expenses Tracker Logo" width="150" height="150">
  
  # Expenses Tracker App

  <p align="center">
    A smart, modern, and intuitive expense tracking application built with Flutter. <br>
    Track your expenses manually or let our AI handle it using Voice Commands!
  </p>

  <!-- Badges -->
  <p align="center">
    <a href="https://play.google.com/store/apps/details?id=com.mohamed.moneyflow&pcampaignid=web_share"><img src="https://img.shields.io/badge/Google_Play-414141?style=for-the-badge&logo=google-play&logoColor=white" alt="Get it on Google Play" /></a>
    <img src="https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter" />
    <img src="https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white" alt="Dart" />
    <img src="https://img.shields.io/badge/Architecture-Clean%20Architecture-brightgreen?style=for-the-badge" alt="Clean Architecture" />
  </p>
</div>

---

## 🎥 App Preview

<p align="center">
  <a href="https://drive.google.com/file/d/1zMZc0EmVLviTO2jI72JsmuQ13Twgh5Tn/view?usp=sharing" target="_blank">
    <img src="https://via.placeholder.com/800x450.png?text=Click+Here+to+Watch+the+Video+on+Google+Drive" alt="Watch the video" width="600"/>
  </a>
  <br>
  <em>(Click the image above to watch the app preview on Google Drive)</em>
</p>

---

## 📖 About The Project

The **Expenses Tracker** is a comprehensive mobile application designed to help users efficiently manage their daily finances. What sets this app apart is its integration of **Artificial Intelligence** through Google's Generative AI, enabling users to log their expenses purely via voice commands in natural language.

Developed with clean architecture and modern Flutter state management practices, it serves as an excellent demonstration of building scalable, maintainable, and feature-rich production applications.

---

## ✨ Key Features

- **🎤 AI-Powered Voice Inputs:** Log your expenses simply by speaking. Integrated with Google Generative AI (Gemini) and Speech-to-Text to parse amounts, categories, and descriptions automatically.
- **📊 Beautiful Analytics & Charts:** Visualize your spending habits through interactive and beautifully designed charts using `fl_chart`.
- **🗂️ Categorization:** Manage, add, and organize your expenses into tailored categories.
- **💾 Offline-First Approach:** Complete local storage implementation using `Hive` to ensure the app works seamlessly without an internet connection.
- **🔐 Secure Authentication:** Secure user authentication flow and encrypted local storage using `flutter_secure_storage`.
- **🌗 Adaptive Theming:** Support for Dark & Light modes with seamless animated transitions.
- **🎨 Modern UI/UX:** Built with a focus on a premium user experience utilizing skeleton loading (shimmer effects), custom animations, and clean layouts.

---

## 🛠️ Tech Stack & Architecture

This project strictly adheres to **Clean Architecture** principles to separate business logic from UI, making the codebase highly testable and maintainable.

### Core Architecture
- **State Management:** `flutter_bloc`
- **Dependency Injection:** `get_it`
- **Functional Programming (Error Handling):** `dartz`
- **Routing:** Standard Flutter Navigator / Modals

### Key Packages
- **Local Database:** `hive`, `hive_flutter`
- **Networking:** `dio`
- **AI / NLP:** `google_generative_ai`, `speech_to_text`, `string_similarity`
- **UI Components:** `fl_chart`, `shimmer`, `loading_animation_widget`, `awesome_snackbar_content`, `syncfusion_flutter_datepicker`
- **Security:** `flutter_secure_storage`

### 📂 Project Structure
The project is built on a **feature-first** approach combined with **Clean Architecture**:

```text
lib/
 ┣ core/              # Core components (network, error handling, di, utils)
 ┃ ┣ config/          # App configurations & themes
 ┃ ┣ connectivity/    # Network connectivity checkers
 ┃ ┣ di/              # Dependency Injection setup
 ┃ ┣ error/           # Error handling & exceptions
 ┃ ┣ network/         # API & networking (Dio) setup
 ┃ ┣ services/        # Third-party services integration
 ┃ ┗ utils/           # Helper functions & constants
 ┣ features/          # Feature-based modules (Clean Architecture)
 ┃ ┣ add_expense/     
 ┃ ┣ auth/
 ┃ ┣ home/
 ┃ ┣ reports/
 ┃ ┣ voice_expense/   # AI Voice Expense functionality
 ┃ ┗ ... (other features)
 ┣ l10n/              # Localization files
 ┣ translation/       # App translations setup
 ┗ main.dart          # Entry point
```

---

## 🚀 Getting Started

Follow these steps to set up the project locally on your machine.

### Prerequisites

- Flutter SDK `^3.7.0` or higher ([Install Flutter](https://docs.flutter.dev/get-started/install))
- Android Studio / VS Code
- A valid Google Gemini API Key (for Voice Expense features)

### Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/your-username/expenses_tracker.git
   cd expenses_tracker
   ```

2. **Fetch dependencies:**
   ```sh
   flutter pub get
   ```

3. **Code Generation:**
   Since the project uses code generators, run the build runner to generate the necessary files (if applicable):
   ```sh
   flutter pub run build_runner build --delete-conflicting-outputs
   ```

4. **Setup Environment / API Keys:**
   Ensure you configure your Google Generative AI API key in the respective environment file or data source before running the voice expense features.

5. **Run the App:**
   ```sh
   flutter run
   ```

---

## 🤝 Contact & Connect

**Email:** [mohamedabdoosman12@gmail.com](mailto:mohamedabdoosman12@gmail.com)

**Download App:** [Money Flow on Google Play Store](https://play.google.com/store/apps/details?id=com.mohamed.moneyflow&pcampaignid=web_share)

---

<p align="center">Made with ❤️ using Flutter</p>
