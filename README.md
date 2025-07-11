# ⏱️ TrackMate - Cross-Platform Time Tracking App

**TrackMate** is a powerful, cross-platform time tracking app built with [Flutter](https://flutter.dev/). It helps you easily log, manage, and sync your work hours across all your devices — perfect for developers and teams using GitHub or GitLab.

---

## 🚀 Features

- ✅ **Cross-platform**: Runs on iOS, Android, Windows, macOS, and Linux  
- 🕒 **Time tracking**: Manually or automatically log work sessions  
- ☁️ **Sync across devices**: All entries are securely synced between devices  
- 🔐 **OIDC login**: Secure authentication using OpenID Connect  
- 🗃️ **Local database**: Time entries are stored locally and synced in the background  
- 🔗 **Issue integration**:
  - Assign time entries to **GitHub** or **GitLab** issues  
  - Automatically log time to issues upon completion  

---

## 📸 Screenshots

*Screenshots of the app will soon be here*

---

## 🛠️ Installation

### Requirements

- Flutter SDK: [Installation Guide](https://docs.flutter.dev/get-started/install)  
- GitHub or GitLab account  
- OIDC-compatible identity provider (e.g. Auth0, Keycloak)

### Build & Run

```bash
# Clone the repository
git clone https://github.com/GeorgRohrhofer/TrackMate.git
cd TrackMate

# Install dependencies
flutter pub get

# Run the app
flutter run
```

---

## 🔗 GitHub & GitLab Integration

1. Sign in via OIDC  
2. Connect your GitHub and/or GitLab account in the app settings  
3. Assign time entries to issues during or after tracking  
4. Upon marking an entry as completed, time is automatically booked to the associated issue

---

## 🧠 Architecture

- **Frontend**: Flutter (Dart)  
- **Storage**: Local database (e.g. SQLite, Hive)  
- **Sync**: Device-to-cloud sync via API or third-party backend  
- **Authentication**: OpenID Connect (OIDC)

---

## 🔒 Security

- OIDC-based secure login  
- Encrypted local storage  
- Secure data transmission via HTTPS

---

## 📦 Deployment

*You can add instructions here for building native binaries for desktop or publishing to app stores.*

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

## 👤 Author

**Georg Rohrhofer**    
[GitHub Profile](https://github.com/GeorgRohrhofer)
