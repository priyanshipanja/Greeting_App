# Greeting App – Personalized Welcome Screen

![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Material Design](https://img.shields.io/badge/Material_Design_3-757575?style=flat-square&logo=material-design&logoColor=white)

A simple two-screen Android app that takes the user's name as input and displays a personalized greeting on a welcome screen. Built with Java, ConstraintLayout, and Material Design 3 — demonstrates Intent-based data passing between activities.

---

## Features

- **Name Input Screen:** Clean dark-themed form with a styled EditText and Submit button.
- **Personalized Greeting:** Passes the entered name via Intent extras to a second activity that displays a custom "Hello, [Name]!" message.
- **Input Validation:** Shows a Toast if the user tries to submit without entering a name.
- **Back Navigation:** Dedicated "Go Back" button on the welcome screen to return to the input screen.
- **Edge-to-Edge UI:** Uses `EdgeToEdge` API for immersive full-screen layout with proper system bar inset handling.
- **Dark Theme Design:** Deep navy background (#021057) with gold accents and light text for a polished look.

---

## Tech Stack

| Component | Technology |
|---|---|
| Language | Java |
| UI | ConstraintLayout, Material Design 3 |
| Min SDK | 24 (Android 7.0) |
| Target SDK | 36 |

---

## Project Structure

```
app/src/main/
├── java/com/priyanshi/greeting_app/
│   ├── MainActivity.java          # Name input + submit logic
│   └── WelcomeActivity.java       # Personalized greeting display
├── res/
│   ├── layout/
│   │   ├── activity_main.xml      # Input screen layout
│   │   └── activity_wellcome.xml  # Welcome screen layout
│   ├── drawable/
│   │   ├── edittext_bg.xml        # Rounded EditText background
│   │   ├── ic_launcher_background.xml
│   │   └── ic_launcher_foreground.xml
│   └── values/
│       ├── colors.xml
│       ├── strings.xml
│       └── themes.xml
└── AndroidManifest.xml
```

---

## Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/priyanshipanja/Greeting-App.git
   ```

2. **Open in Android Studio**
   - File → Open → select the project root

3. **Run the app**
   - Connect a device or start an emulator (API 24+)
   - Click ▶ Run

---

## How It Works

```
MainActivity                    WelcomeActivity
┌──────────────┐   Intent +    ┌──────────────────┐
│ Enter Name   │──"username"──▶│ Hello, [Name]!   │
│ [Submit]     │               │ Welcome message  │
│              │◀──finish()────│ [Go Back]        │
└──────────────┘               └──────────────────┘
```

---

## License

MIT © [Priyanshi Panja](https://github.com/priyanshipanja)
