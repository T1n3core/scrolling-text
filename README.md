# Scrolling Text – Android App

## About the Project

This project was developed as part of **Mobile Application Development – Assignment 4**. The goal is to create a scrollable article layout with two columns: a narrower left column for the subtitle and a wider right column for the main article text.

The application demonstrates how to display long-form text in a mobile interface using Android UI components, with a focus on layout organization, text readability, and vertical scrolling.

The application is developed in **Java** using **Android Studio**, with the user interface defined in XML.

## Features

- Scrollable article containing multiple paragraphs of text.
- Two-column text layout:
  - Narrow left column for the subtitle.
  - Wider right column for the main article.
- Horizontal `LinearLayout` to position the two text columns side by side.
- `ScrollView` to support vertical scrolling through the article.
- Text resources stored in `strings.xml` for easier content management and localization.
- Comment button positioned at the bottom of the interface.
- Toast notification displaying `Comment submitted!` when the button is clicked.

## Technologies Used

- **Language:** Java
- **IDE:** Android Studio
- **UI Design:** XML
- **Platform:** Android
- **Components:** TextView, ScrollView, LinearLayout, Button, Toast
- **Resources:** `strings.xml`

## Application Structure

The application primarily uses the following files:

- `activity_main.xml` – Defines the user interface, including the scrollable article, two-column layout, and comment button.
- `MainActivity.java` – Handles user interactions and displays a Toast notification when the comment button is clicked.
- `strings.xml` – Stores the article title, subtitle, and main article text as string resources.

## How It Works

1. Launch the application to display the article.
2. The subtitle appears in a narrow column on the left side of the screen.
3. The main article text appears in a wider column on the right.
4. Scroll vertically to read the entire article.
5. Tap the **Comment** button at the bottom of the interface.
6. A Toast notification displays `Comment submitted!`.

## Layout Design

The application uses a `ScrollView` containing a single `LinearLayout` with a horizontal orientation. The `LinearLayout` contains two `TextView` components, one for the subtitle and one for the main article.

The left column has a fixed width of `100dp`, while the right column occupies the remaining available space. This arrangement allows the subtitle to wrap across multiple lines while providing sufficient space for the main article.

The article is long enough to exceed the available screen height, allowing the user to navigate through the content using vertical scrolling.

## Installation and Setup

1. Clone this repository:

   ```bash
   git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
   ```

2. Open **Android Studio**.
3. Select **Open** and choose the cloned project folder.
4. Wait for Gradle to finish syncing.
5. Start an Android emulator or connect an Android device.
6. Click **Run** to build and launch the application.

Replace `YOUR-USERNAME` and `YOUR-REPOSITORY` with your GitHub username and repository name.

## Learning Objectives

This assignment provides practical experience with:

- Designing Android user interfaces using XML.
- Displaying long-form text using `TextView`.
- Implementing vertical scrolling with `ScrollView`.
- Organizing UI components using `LinearLayout`.
- Creating horizontal layouts with multiple columns.
- Controlling component dimensions using layout attributes such as `layout_width`.
- Managing text content through string resources in `strings.xml`.
- Handling button clicks and displaying feedback using Toast notifications.
- Understanding the requirement that a `ScrollView` must contain exactly one direct child view.
