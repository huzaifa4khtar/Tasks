
<p align="center">
  <img src="media/tasks_logo_transparent.png" width="200" alt="Tasks Logo" />
</p>

<p align="center">
Tasks lets you manage your tasks, lists, and schedules, set reminders, and run focused work sessions with live timers.<br>
Create a free account and your data syncs securely across devices with cloud storage.
</p>

<p align="center">
  <a href="https://github.com/huzaifa4khtar/Tasks/releases/download/v1.0.0/Tasks-Setup-v1.0.0.apk"><img src="https://img.shields.io/badge/Download-Tasks_v1.0.0-0077B6?style=for-the-badge&logo=android&logoColor=white" alt="Download" /></a>
</p>

<p align="center">
  <a href="mailto:huzaifa4khtar@gmail.com"><img src="https://img.shields.io/badge/Support-Email-DB4437?style=for-the-badge&logo=gmail&logoColor=white" alt="Support" /></a>
  <a href="https://linkedin.com/in/huzaifa4khtar"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
</p>

<p align="center">
  <a href="https://glasneph.github.io/tasks_legal_documentation/privacy_policy.html"><img src="https://img.shields.io/badge/Privacy_Policy-555555?style=for-the-badge" alt="Privacy Policy" /></a>
  <a href="https://glasneph.github.io/tasks_legal_documentation/terms_and_conditions.html"><img src="https://img.shields.io/badge/Terms_&_Conditions-555555?style=for-the-badge" alt="Terms & Conditions" /></a>
  <a href="https://glasneph.github.io/tasks_legal_documentation/end_user_license_agreement.html"><img src="https://img.shields.io/badge/EULA-555555?style=for-the-badge" alt="EULA" /></a>
  <a href="https://github.com/huzaifa4khtar/Tasks/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-AGPL--3.0-blue?style=for-the-badge" alt="License" /></a>
</p>

<br/>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#introduction">Introduction</a></li>
    <li><a href="#tech-stack">Tech Stack</a></li>
    <li><a href="#features">Features</a></li>
    <li><a href="#project-structure">Project Structure</a></li>
    <li><a href="#requirements">Requirements</a></li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#for-users">For Users</a></li>
        <li><a href="#for-developers">For Developers</a></li>
      </ul>
    </li>
    <li>
      <a href="#contributing">Contributing</a>
      <ul>
        <li><a href="#how-to-contribute">How to Contribute</a></li>
        <li><a href="#top-contributors">Top Contributors</a></li>
      </ul>
    </li>
    <li><a href="#author">Author</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#ui-screenshots">UI Screenshots</a></li>
  </ol>
</details>

<br/>

## Introduction

We all have busy lives, work deadlines, study sessions, and a hundred things to keep track of. **Tasks** was built to make that a little easier. It's a user friendly app where you can jot down your tasks, give them due dates and times, mark them as important, and organize them into your own custom lists. You'll get reminded when tasks are due or missed, so nothing slips through the cracks.

But Tasks isn't just a todo list. It also has **Sessions**, think of them as Pomodoro style work blocks where you pick the tasks you want to tackle, set how long each one takes, and the app keeps you on track with a timer and notification during sessions and upon completion.

Everything syncs to a cloud storage, so your data is always safe and available across devices. You can sign up with your email or just use Google Sign-In. The whole thing is wrapped in a soft, glassmorphic design, not boring corporate look. And the best part? It's completely free. No ads, no subscriptions, no data selling. Just a tool that works.

<br/>

## Tech Stack

| Layer | Technology |
|-------|-----------|
| **Framework** | [![Flutter][Flutter-shield]][Flutter-url] [![Dart][Dart-shield]][Dart-url] |
| **Design** | [![Google Stitch][Stitch-shield]][Stitch-url] |
| **State Management** | [![Riverpod][Riverpod-shield]][Riverpod-url] |
| **Backend** | [![Firebase][Firebase-shield]][Firebase-url] |
| **Database** | [![Firestore][Firestore-shield]][Firestore-url] |
| **Authentication** | [![Firebase Auth][Auth-shield]][Auth-url] [![Google Sign-In][Google-shield]][Google-url] |
| **Notifications** | [![awesome_notifications][Notif-shield]][Notif-url] |
| **Navigation** | [![curved_navigation_bar][Nav-shield]][Nav-url] |
| **Icons** | [![font_awesome_flutter][FA-shield]][FA-url] |

<br/>

## Features

| Feature | Description |
|---------|-------------|
| **Task Management** | Create, edit, delete, and toggle tasks with due dates, times, and importance flags |
| **Categories** | Sort tasks by Study, Work, or Home, plus create your own custom lists with range of icons and colors |
| **Smart Reminders** | Get notified 12 hours before, 2 hours before, and when a task is missed |
| **Focused Sessions** | Build work sessions with multiple tasks and breaks, run them with a live timer |
| **Profile & Stats** | Choose an avatar, edit your name, and track tasks completed and sessions finished |
| **Custom Lists** | Create your own task categories with custom icons and colors |
| **Authentication** | Sign up with email/password or Google Sign-In, with email verification |
| **Account Management** | Update your email, change your password, or delete your account |
| **Legal Pages** | Privacy Policy, Terms & Conditions, and EULA accessible in-app |

<br/>

## Project Structure

```
Tasks/
├── app/                        # Flutter application
│   ├── lib/
│   │   ├── main.dart           # Entry point, Firebase init, AuthGate
│   │   ├── constants.dart      # Design system (colors, text, spacing)
│   │   ├── models/             # Data models: Task, Session
│   │   ├── providers/          # Riverpod providers: auth, services, session
│   │   ├── screens/            # 20 screens (home, login, profile, etc.)
│   │   ├── services/           # 5 services: auth, task, session, reminder, notification
│   │   └── widgets/            # 14 reusable UI components
│   ├── assets/                 # Logos, avatars, fonts
│   ├── functions/              # Cloud Functions (TypeScript)
│   ├── android/                # Android project
│   ├── test/                   # Unit tests
│   └── pubspec.yaml            # Dependencies
├── media/                      # App logo and UI screenshots
│   ├── tasks_logo_transparent.png
│   └── ui_screenshots/         # 29 UI screenshots
├── LICENSE                     # AGPL-3.0
├── DESIGN.md                   # Design system document
└── README.md
```

<br/>

## Requirements

| Requirement | Minimum |
|-------------|---------|
| Android Version | 7.0 (API 24) or higher |
| RAM | 1-2 GB |
| Storage | ~85 MB |
| Network | Required (for cloud sync and authentication) |

<br/>

## Getting Started

### For Users

1. [Download](https://github.com/huzaifa4khtar/Tasks/releases/download/v1.0.0/Tasks-Setup-v1.0.0.apk) the Latest APK.
2. Install the APK on your Android device
3. Launch Tasks from your app drawer
4. Sign up with email or Google Sign-In to start managing your tasks

> **Note:** Your device may show a Google Play warning when installing the APK. This is because the app is distributed outside the Play Store, not because it's infected. Tasks is completely open-source, feel free to inspect the code before installing this application. Tap **"Install anyway"** when prompted. Alternatively, you can disable Play Protect temporarily by opening the **Play Store app** → tap your **profile icon** (top right) → **Play Protect** → **Settings** → toggle **"Scan apps with Play Protect"** off. Turn it back on once the application is installed.

### For Developers

**Prerequisites:**
- [Flutter SDK](https://docs.flutter.dev/get-started/install)
- [Firebase CLI](https://firebase.google.com/docs/cli)
- [Firebase project](https://console.firebase.google.com/)

**Setup:**

```bash
# 1. Clone the repository
git clone https://github.com/huzaifa4khtar/Tasks.git
cd Tasks/app

# 2. Install dependencies
flutter pub get

# 3. Configure Firebase
# Place your google-services.json in android/app/
# Or run: flutterfire configure

# 4. Run the app
flutter run
```

**Build:**

```bash
# Android APK
flutter build apk --release --no-tree-shake-icons
```

```bash
# Android AAB (For Google PlayStore)
flutter build appbundle --release --no-tree-shake-icons
```

> **Note:** This project uses dynamic IconData construction for custom list icons (code points stored in Firestore), which prevents Flutter's icon tree-shaking from working. You must use `--no-tree-shake-icons` when building APK or AAB.

**Run tests:**

```bash
cd app
flutter test
```

<br/>

## Contributing

If you want to contribute to this project, you are more than welcome to do so. Together we can make this tool even more helpful.

### How to Contribute

1. **Fork the repository**
   ```bash
   # Click the "Fork" button on the top right of the repo page
   ```

2. **Clone your fork**
   ```bash
   git clone https://github.com/<your-username>/Tasks.git
   cd Tasks
   ```

3. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

4. **Make your changes**
   - Follow the existing code style and conventions
   - Keep changes focused, one feature or fix per PR
   - Test your changes before committing

5. **Build and verify**
   ```bash
   cd app
   flutter test
   flutter analyze
   ```

6. **Commit your changes**
   ```bash
   git add .
   git commit -m "Add: brief description of your change"
   ```

7. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

8. **Open a Pull Request**
   - Go to the original repo and click "New Pull Request"
   - Select your feature branch
   - Provide a clear title and description of your changes
   - Reference any related issues

### Top Contributors

<a href="https://github.com/huzaifa4khtar/Tasks/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=huzaifa4khtar/Tasks" alt="contrib.rocks image" />
</a>

<br/>
<br/>

## Author

**Muhammad Huzaifa**

<a href="https://github.com/huzaifa4khtar"><img src="https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
<a href="https://linkedin.com/in/huzaifa4khtar"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
<a href="mailto:huzaifa4khtar@gmail.com"><img src="https://img.shields.io/badge/Email-Contact-DB4437?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>

<br/>

## Acknowledgements

I would like to thank the following resources and individuals:

- [Magnific](https://magnific.com) for profile avatar images.
- [shields.io](https://shields.io/) for badge images used in this README.
- [contrib.rocks](https://contrib.rocks) for auto-generated contributor avatars.
- [Best-README-Template](https://github.com/othneildrew/Best-README-Template) for the README structure reference.

A special thanks to all the devs and contributors of the packages, tools, and frameworks listed in the <a href="#tech-stack">Tech Stack</a> section.

<br/>

## License

This project is licensed under the [GNU Affero General Public License v3.0](LICENSE).

<br/>

## UI Screenshots

<table>
  <tr>
    <td><img src="media/ui_screenshots/01_app_launcher.png" width="250"></td>
    <td><img src="media/ui_screenshots/02_sineup_screen.png" width="250"></td>
    <td><img src="media/ui_screenshots/03_login_screen.png" width="250"></td>
  </tr>
  <tr>
    <td><img src="media/ui_screenshots/04_home_screen.png" width="250"></td>
    <td><img src="media/ui_screenshots/05_adding_tasks.png" width="250"></td>
    <td><img src="media/ui_screenshots/06_task_list.png" width="250"></td>
  </tr>
  <tr>
    <td><img src="media/ui_screenshots/07_task_12h_remainder.png" width="250"></td>
    <td><img src="media/ui_screenshots/08_task_2h_remainder.png" width="250"></td>
    <td><img src="media/ui_screenshots/09_task_missed_remainder.png" width="250"></td>
  </tr>
  <tr>
    <td><img src="media/ui_screenshots/10_remainder_screen.png" width="250"></td>
    <td><img src="media/ui_screenshots/11_profile_screen.png" width="250"></td>
    <td><img src="media/ui_screenshots/12_profile_edit_screen_1.png" width="250"></td>
  </tr>
  <tr>
    <td><img src="media/ui_screenshots/13_profile_edit_screen_2.png" width="250"></td>
    <td><img src="media/ui_screenshots/14_my_list_screen.png" width="250"></td>
    <td><img src="media/ui_screenshots/15_adding_custom_list.png" width="250"></td>
  </tr>
  <tr>
    <td><img src="media/ui_screenshots/16_all_list_expandable_section.png" width="250"></td>
    <td><img src="media/ui_screenshots/17_session_screen.png" width="250"></td>
    <td><img src="media/ui_screenshots/18_creating_editing_session.png" width="250"></td>
  </tr>
  <tr>
    <td><img src="media/ui_screenshots/19_active_session_task.png" width="250"></td>
    <td><img src="media/ui_screenshots/20_active_session_break.png" width="250"></td>
    <td><img src="media/ui_screenshots/21_active_session_timer_notification.png" width="250"></td>
  </tr>
  <tr>
    <td><img src="media/ui_screenshots/22_session_complete_notification.png" width="250"></td>
    <td><img src="media/ui_screenshots/23_settings_screen.png" width="250"></td>
    <td><img src="media/ui_screenshots/24_manage_account_screen.png" width="250"></td>
  </tr>
  <tr>
    <td><img src="media/ui_screenshots/25_update_email_screen.png" width="250"></td>
    <td><img src="media/ui_screenshots/26_update_password_screen.png" width="250"></td>
    <td><img src="media/ui_screenshots/27_reset_password_screen.png" width="250"></td>
  </tr>
  <tr>
    <td><img src="media/ui_screenshots/28_delete_account_screen.png" width="250"></td>
    <td><img src="media/ui_screenshots/29_faq_screen.png" width="250"></td>
    <td></td>
  </tr>
</table>

<!-- MARKDOWN LINKS & IMAGES -->
[Flutter-shield]: https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white
[Flutter-url]: https://flutter.dev
[Dart-shield]: https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white
[Dart-url]: https://dart.dev
[Firebase-shield]: https://img.shields.io/badge/Firebase-DD2C00?style=for-the-badge&logo=firebase&logoColor=white
[Firebase-url]: https://firebase.google.com
[Firestore-shield]: https://img.shields.io/badge/Firestore-FFCA28?style=for-the-badge&logo=firebase&logoColor=black
[Firestore-url]: https://firebase.google.com/docs/firestore
[Auth-shield]: https://img.shields.io/badge/Firebase_Auth-DD2C00?style=for-the-badge&logo=firebase&logoColor=white
[Auth-url]: https://firebase.google.com/docs/auth
[Google-shield]: https://img.shields.io/badge/Google_Sign--In-4285F4?style=for-the-badge&logo=google&logoColor=white
[Google-url]: https://developers.google.com/identity/sign-in/web/sign-in
[Riverpod-shield]: https://img.shields.io/badge/Riverpod-0040FF?style=for-the-badge&logo=dart&logoColor=white
[Riverpod-url]: https://riverpod.dev
[Notif-shield]: https://img.shields.io/badge/awesome__notifications-02569B?style=for-the-badge&logo=flutter&logoColor=white
[Notif-url]: https://pub.dev/packages/awesome_notifications
[Nav-shield]: https://img.shields.io/badge/curved__navigation__bar-02569B?style=for-the-badge&logo=flutter&logoColor=white
[Nav-url]: https://pub.dev/packages/curved_navigation_bar
[FA-shield]: https://img.shields.io/badge/font__awesome__flutter-339AF0?style=for-the-badge&logo=fontawesome&logoColor=white
[FA-url]: https://pub.dev/packages/font_awesome_flutter
[Stitch-shield]: https://img.shields.io/badge/Google_Stitch-555555?style=for-the-badge&logo=google&logoColor=white
[Stitch-url]: https://stitch.withgoogle.com
