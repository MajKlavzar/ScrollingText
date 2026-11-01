# ScrollingText - Working with Text and Scroll Views

An Android application demonstrating how to display long articles (*The Beatles Anthology*) using a two-column layout wrapped inside a `ScrollView`. Created as an Android SDK development exercise to practice working with `TextView`, `ScrollView`, `LinearLayout`, and `ConstraintLayout`.

---

## 📱 App Overview

The application displays a long article in a clean, readable two-column layout on mobile devices:
- **Article Heading**: Displayed at the top of the screen in bold text (`The Beatles Anthology`).
- **Two-Column Text Display**:
  - **Left Column (Subheadings)**: A narrower column (`100dp`) with bold text for section subheadings and song titles.
  - **Right Column (Main Content)**: A wider column (`layout_weight="1"`) taking up the remaining screen width to display the article paragraphs.
- **Vertical Scrolling**: All content is enclosed in a `ScrollView` for smooth scrolling throughout the entire article.
- **Interactive Button**: Positioned at the bottom center of the screen (*Add Comment*), displaying a `Toast` notification saying *"Comment submitted!"* when clicked.

---

## 🛠️ Technologies & UI Components

- **Language & Framework**: Java / Android SDK
- **User Interface (XML)**:
  - `ConstraintLayout`: Root layout container for the screen.
  - `ScrollView`: Scrollable container holding exactly one direct child container (`LinearLayout`).
  - `LinearLayout`: Horizontally oriented layout (`android:orientation="horizontal"`) pairing left subheadings with right paragraphs.
  - `TextView`: UI elements displaying heading, subheadings, and article text.
  - `Button`: Action button pinned to the bottom center.
  - `Toast`: Temporary notification popup triggered by button click.
- **Resources**: All string literals are managed in `strings.xml`.

---

## 📂 Project Structure

```
ScrollingText/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/scrollingtext/
│   │   │   │   └── MainActivity.java          # Main activity logic & click handlers
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   │   └── activity_main.xml      # Main screen layout
│   │   │   │   └── values/
│   │   │   │       ├── colors.xml             # Color resources
│   │   │   │       ├── strings.xml            # String resources
│   │   │   │       └── themes.xml             # Theme configuration
│   │   └── test/                              # Unit tests
│   └── build.gradle.kts                       # Module-level Gradle configuration
└── README.md                                  # Project documentation
```

---

## 🚀 How to Run

1. Open the project in **Android Studio**.
2. Wait for **Gradle Sync** to finish.
3. Run the application on an Android Emulator or physical device by clicking **Run (Shift + F10)**.
