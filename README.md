# belajar-native

A React Native application built with Expo that allows users to pick images and add emoji stickers to them.

## Features

*   Pick images from the device's gallery.
*   Display selected images.
*   Choose from a list of emojis.
*   Add selected emojis as stickers onto the image.
*   Tab-based navigation for different sections of the app (e.g., Home, About).

## Prerequisites

*   Node.js (LTS version recommended) - includes npm. You can download it from [nodejs.org](https://nodejs.org/).
*   Expo CLI:
    ```bash
    npm install -g expo-cli
    ```
*   A mobile development environment:
    *   For iOS development: macOS with Xcode.
    *   For Android development: Android Studio and JDK.
    *   Alternatively, you can use the [Expo Go app](https://expo.dev/go) on a physical iOS or Android device for testing and development.

## Getting Started / Installation

1.  **Clone the repository:**
    ```bash
    git clone <your-repository-url> # Replace <your-repository-url> with the actual URL
    cd belajar-native
    ```

2.  **Install dependencies:**
    Using npm:
    ```bash
    npm install
    ```
    Or using yarn:
    ```bash
    yarn install
    ```

## Available Scripts

The following scripts are available from the project's `package.json`:

*   `npm start` or `npx expo start`
    *   Starts the Metro bundler and development server. Provides options to open the app in an emulator/simulator or on a physical device via the Expo Go app.

*   `npm run android` or `npx expo start --android`
    *   Builds and runs the app on a connected Android device or emulator.

*   `npm run ios` or `npx expo start --ios`
    *   Builds and runs the app on an iOS simulator (or a connected device if properly configured).

*   `npm run web` or `npx expo start --web`
    *   Bundles the app for the web and serves it in a browser.

*   `npm run lint` or `npx expo lint`
    *   Lints the project files using ESLint to check for code quality and style issues.

*   `npm run reset-project`
    *   This command (if you keep the script from the initial Expo setup) moves the starter code to an `app-example` directory and creates a blank `app` directory. Useful if you want to start over from a clean slate while keeping the example code.

## Tech Stack

*   **Core:**
    *   React Native
    *   Expo SDK
    *   TypeScript
*   **Navigation:**
    *   Expo Router
    *   React Navigation (underlying library)
*   **UI & Interaction:**
    *   React Native Gesture Handler
    *   React Native Reanimated
*   **Utilities & Features:**
    *   Expo Image Picker
    *   Expo Vector Icons
    *   Expo Font
    *   Expo Status Bar
    *   Expo Splash Screen
    *   Expo Haptics
    *   Expo System UI
*   **Linting:**
    *   ESLint (`eslint-config-expo`)

## File Structure Overview

A brief overview of some key directories:

*   `app/`: Contains the application's screens and navigation logic, powered by Expo Router.
    *   `(tabs)/`: Defines the layout and screens for the tab-based navigation (e.g., `index.tsx` for the main screen, `about.tsx` for an about screen).
    *   `_layout.tsx`: The root layout component for the entire application.
    *   `+not-found.tsx`: A component to handle routes that don't match any defined screen.
*   `assets/`: Stores static assets like images, fonts, etc.
    *   `images/`: Contains image files used in the app (icons, backgrounds, emojis, etc.).
    *   `fonts/`: Contains custom font files (e.g., `SpaceMono-Regular.ttf`).
*   `components/`: Houses reusable UI components used across different screens (e.g., `ImageViewer.tsx`, `Button.tsx`, `EmojiPicker.tsx`).
*   `node_modules/`: Directory where all project dependencies (npm packages) are installed.
*   `.vscode/`: Contains editor-specific settings for Visual Studio Code (e.g., `settings.json`).

## Learn More (Expo Resources)

To learn more about developing your project with Expo, look at the following resources:

*   [Expo Documentation](https://docs.expo.dev/): Learn fundamentals, or go into advanced topics with guides.
*   [Learn Expo Tutorial](https://docs.expo.dev/tutorial/introduction/): Follow a step-by-step tutorial.
*   [Expo on GitHub](https://github.com/expo/expo): View the open-source platform and contribute.
*   [Discord Community](https://chat.expo.dev): Chat with Expo users and ask questions.

---

_This README was generated based on the project structure and dependencies._
