# ⏱️ TimeSync - Cross-Platform Time Tracking App

**TimeSync** ist eine leistungsstarke und plattformübergreifende Time-Tracking-App, entwickelt mit [Flutter](https://flutter.dev/). Sie ermöglicht das einfache Erfassen, Verwalten und automatische Synchronisieren von Arbeitszeiten – ideal für Entwickler:innen und Teams, die mit GitHub oder GitLab arbeiten.

---

## 🚀 Features

- ✅ **Plattformübergreifend**: Funktioniert auf iOS, Android, Windows, macOS und Linux  
- 🗓️ **Zeiterfassung**: Manuelles oder automatisches Tracken von Arbeitszeiten  
- ☁️ **Synchronisierung**: Einträge werden geräteübergreifend synchronisiert  
- 🔒 **Login via OIDC**: Sicheres Einloggen über OpenID Connect  
- 🗃️ **Datenbankbasiert**: Alle Einträge werden lokal gespeichert und synchronisiert  
- 🔗 **Issue-Integration**:
  - Verknüpfe Time-Tracking-Einträge mit **GitHub**- oder **GitLab-Issues**
  - **Automatisches Buchen** der Zeiten auf Issues nach Abschluss

---

## 📸 Screenshots

*Hier könnten ein paar Screenshots der App eingefügt werden.*

---

## 🛠️ Installation

### Voraussetzungen

- Flutter SDK: [Installationsanleitung](https://docs.flutter.dev/get-started/install)  
- GitHub/GitLab Account mit Zugriff auf Issues  
- OIDC-kompatibler Identity Provider (z. B. Auth0, Keycloak)

### Build & Run

```bash
# Repository klonen
git clone https://github.com/dein-benutzername/timesync.git
cd timesync

# Abhängigkeiten installieren
flutter pub get

# App starten
flutter run
```

---

## 🔗 Integration mit GitHub & GitLab

1. Logge dich über OIDC ein.
2. Verknüpfe deine GitHub- und/oder GitLab-Konten in den App-Einstellungen.
3. Time-Tracking-Einträge können Issues zugewiesen werden.
4. Beim Markieren eines Eintrags als "abgeschlossen" wird die Zeit automatisch auf das verknüpfte Issue gebucht.

---

## 🧠 Architektur

- **Frontend**: Flutter (Dart)  
- **Storage**: Lokale Datenbank (z. B. SQLite oder Hive)  
- **Sync**: Cloud-Synchronisierung über eigene API oder Drittanbieter (abhängig vom Setup)  
- **Auth**: OpenID Connect (OIDC)

---

## 🔒 Sicherheit

- Authentifizierung über OIDC (z. B. Keycloak, Auth0)  
- Lokale Daten verschlüsselt gespeichert  
- Gesicherte Synchronisation (HTTPS/SSL)

---

## 📦 Deployment

*Optionaler Abschnitt für Desktop/Mobile Builds oder Deployment-Targets.*

---

## 🤝 Beitrag leisten

Pull Requests und Feedback sind willkommen!

1. Forke das Projekt
2. Erstelle deinen Feature-Branch (`git checkout -b feature/DeinFeature`)
3. Commit deine Änderungen (`git commit -m 'Feature hinzufügen'`)
4. Push auf den Branch (`git push origin feature/DeinFeature`)
5. Erstelle einen Pull Request

---

## 📄 Lizenz

Dieses Projekt steht unter der MIT-Lizenz – siehe [LICENSE](LICENSE) für Details.

---

## 👤 Autor

**Dein Name oder Team**  
[deine-website.dev](https://deine-website.dev)  
[GitHub Profil](https://github.com/dein-benutzername)

---

## 📬 Kontakt

Bei Fragen oder Feedback gerne ein Issue erstellen oder direkt kontaktieren: [you@example.com](mailto:you@example.com)
