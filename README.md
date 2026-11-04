# Mac-Pan-Pac-Man

## About

Mac-Pan-Pac-Man is a JavaFX-based arcade puzzle game developed as a second-year Bachelor's (L2) project at Université Paris Cité based on the game Pacman. Building upon a base architecture provided by the teaching staff, our team designed, modified, and implemented new features, menus, and multimedia integrations in Java.

The game features classic arcade mechanics combined with an interactive user interface, an intro video sequence, background music, sound effects, level management, and a dynamic multiplayer mode.

*Note: This application has been fully tested and runs natively on Windows. Running the project on Linux or via WSL may require additional audio and multimedia configuration (such as GStreamer packages or specific audio routing) due to JavaFX and Java Sound platform dependencies. The source code and comments might contains some French.*

## Tech Stack

- **Language:** Java (OpenJDK 21)
- **Framework & GUI:** JavaFX (Graphics, Media)
- **Audio:** Java Sound API (`javax.sound.sampled`)
- **Build System:** Gradle
- **Architecture:** Model-View-Controller / Component-based GUI design

## Key Features

**Graphical Interface & Responsive Design:** Built with JavaFX, featuring a custom window layout, adaptive/resizable game views where UI elements dynamically scale and follow screen adjustments, menus, and dedicated game views.
- **Multimedia Integration:** Includes an introductory video sequence (`MediaPlayer` / `MediaView`) and custom audio/music management (`Music` class).
- **Classic Arcade Gameplay & Multiplayer:** Faithful recreation of Pac-Man-style grid movement, featuring both a solo mode and a multiplayer mode (co-op or versus).
- **Level Management:** Structured menus allowing users to transition smoothly from intro to game selection (Solo/Multiplayer modes).
- **Cross-Platform Compatibility Notes:** Tailored handling for platform-specific multimedia and audio codecs (Windows Media Foundation & Linux/WSL GStreamer integration).

## Project Structure

```text
📁 pacman-java-fx
│
├── 📁 config/                      # Global project configuration files
├── 📁 gradle/                      # Gradle wrapper files
├── 📁 src/
│   ├── 📁 main/
│   │   ├── 📁 java/                # Main Java source code
│   │   │   ├── 📁 config/          # Application and maze configurations
│   │   │   ├── 📁 geometry/        # Geometric calculations and coordinate handling
│   │   │   ├── 📁 gui/             # Graphical interfaces, views, and window management
│   │   │   │   ├── 📁 controller/  # Controllers managing user interactions
│   │   │   │   └── 📁 menu/        # Game menus (Solo, Multiplayer, Main Menu)
│   │   │   ├── 📁 misc/            # Miscellaneous classes and helper utilities
│   │   │   ├── 📁 model/           # Data models and core game business logic
│   │   │   └── 📁 utils/           # Utility classes (Resource management, sound, FPS)
│   │   │
│   │   └── 📁 resources/           # Game assets (videos, audio, images, maps)
│   │
│   └── 📁 test/                    # Unit tests for the project
│
├── 📄 build.gradle                 # Gradle build configuration
├── 📄 gradlew / gradlew.bat        # Gradle wrapper execution scripts
└── 📄 README.md                    # Project documentation
```

## Getting Started

### Prerequisites

* Java Development Kit (JDK 21 or compatible)
* Gradle
* OS-specific dependencies:
    * Windows: Standard Windows environment (Media Foundation codecs included).
    * Linux / WSL: Requires some audio/media packages for JavaFX media playback.

## Installation & Execution

1. **Clone the repository:**
```bash
git clone https://github.com/SuyuKuka/pacman-java-fx.git
cd pacman-java-fx
```

2. **Build the project:**
```bash
./gradlew build
```

3. **Launch the game:**
```bash
./gradlew run
```

4. **Cleaning**
```bash
./gradlew clean
```

## Controls

* Player 1 / Solo: Arrow keys
* Player 2: ZQSD or WASD (both layouts are supported)
* Menu Navigation: Arrows keys or mouse clicks or  to interact with buttons (Solo, Multiplayer, Settings, etc.).
* Escape: Quit or return to previous menus.

## Team

This project was developed collaboratively as a 6-person team:

- **CHEN Michel** - Collaborative Java Development & Implementation 
  [![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?logo=github)](https://github.com/SuyuKuka)
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-0A66C2?logo=linkedin)](https://linkedin.com/in/chen-michel)

- **CHIV Henri** - Collaborative Java Development & Implementation 
  [![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?logo=github)](https://github.com/H-flamme)

- **DUONG Viet Thanh** - Collaborative Java Development & Implementation 
  [![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?logo=github)](https://github.com/Tan8520)

- **LIN Qinghui** - Collaborative Development & Implementation 
  [![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?logo=github)](https://github.com/qinghui-lin)

- **LIU Shiqi** - Collaborative Java Development & Implementation 
  [![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?logo=github)](https://github.com/SuyuKuka)

- **Nguyen Duc Vinh** - Collaborative Java Development & Implementation 
  [![GitHub](https://img.shields.io/badge/GitHub-Profile-181717?logo=github)](https://github.com/VHN27)

## License

This repository contains academic coursework.

- The initial basecode are the intellectual property of the teaching staff. They are included here strictly for context and evaluation purposes.
- The core implementations, custom extensions, UI designs, responsive window handling, and gameplay logic are our team's work.

This project is shared for portfolio and reference purposes only.