# Prodev Mobile Setup Repository

This repository contains several tasks that guide you through setting up your mobile development environment and building React Native applications using the Expo framework. Each task demonstrates different aspects of mobile app development—from setting up your environment to implementing complex UI components.

---

## Task 0: Setting Up and Testing Your Mobile Development Environment

**Objective:**  
Set up your mobile development environment with Node.js LTS, VS Code, and Expo Go on your physical device. Document the installation process and any challenges you encounter.

**Steps:**
1. **Install Prerequisites:**
   - Install Node.js LTS.
   - Install VS Code.
   - Ensure you’re running macOS, Linux, or Windows.
2. **Install Expo Go:**
   - Download and install Expo Go
---

## Task 1: Create Your First Mobile App

**Objective:**  
Initialize your first Expo project using the latest Expo Router template, modify the default home screen, and understand the file structure of a React Native application.

**Steps:**
1. **Project Initialization:**
   - Navigate to your project directory:
     ```sh
     cd prodev-mobile-setup
     ```
   - Initialize a new Expo project:
     ```sh
     npx create-expo-app@latest .
     ```
2. **Modify the Home Screen:**
   - Open `app/(tabs)/index.tsx` and change the default text from "Welcome!" to "** First App Created**".
3. **Run and Test:**
   - Start the development server using:
     ```sh
     npx expo start
     ```
   - Scan the QR code with Expo Go (or the Camera app on iOS).
4. **Reset the Application:**
   - Run the reset command:
     ```sh
     npm run reset-project
     ```
---

## Task 2: Implementing Mobile Components in React Native

**Objective:**  
Learn to use essential React Native components like `<View>`, `<Text>`, and `<TouchableOpacity>`, and style them using `StyleSheet`.

**Steps:**
1. **Project Setup:**
   - Initialize a new Expo project in the directory `prodev-mobile-app-0x01`.
   - Reset the project with:
     ```sh
     npm run reset-project
     ```
2. **Update the Home Screen:**
   - Open `app/index.tsx` and change the main `<Text>` component to display "Entry Screen - Awesome".
   - Replace any inline style on the root `<View>` with `style={styles.container}`.
   - Add three additional `<Text>` components within a `<View>`, each styled with `styles.largeText`, `styles.mediumText`, and `styles.smallText`.
3. **Define Styles:**
   - Use `StyleSheet.create` within the same file to define the styles for the container and text components.
4. **Test the App:**
   - Run the application and verify the UI on your physical device.

---

## Task 3: Building a Sample Login Screen Using Core React Native Components

**Objective:**  
Implement a login screen using core React Native components such as `SafeAreaView`, `ImageBackground`, `Image`, `TouchableOpacity`, and others. This task helps reinforce your understanding of layout, styling, and component composition.

**Steps:**
1. **Project Initialization:**
   - Create a new Expo project in the directory `prodev-mobile-app-0x03`:
     ```sh
     npx create-expo-app@latest prodev-mobile-app-0x03
     ```
   - Navigate into the project:
     ```sh
     cd prodev-mobile-app-0x03
     ```
   - Reset the project:
     ```sh
     npm run reset-project
     ```
2. **Asset Management:**
   - Download the required assets (e.g., `logo.png`, `google.png`, `facebook.png`, `splash.png`) and place them in the `assets/images` directory.
3. **Implement Styles:**
   - Create a new file at `styles/index.tsx` and manually type in the style definitions. This file defines styles for the container, text, buttons, input fields, and other UI components.
4. **Configure Layout:**
   - Modify `app/_layout.tsx` to disable the header:
     ```tsx
     import { Stack } from "expo-router";

     export default function RootLayout() {
       return <Stack screenOptions={{ headerShown: false }} />;
     }
     ```
5. **Build the Login Screen:**
   - Update `app/index.tsx` to implement the login screen UI:
     - **Navigation Group:** Contains a back arrow icon and the company logo.
     - **Text Components:** Display a title and descriptive text.
     - **Form Group:** Includes an email input, a password field with an eye icon, and a "Forgot password?" link.
     - **Buttons:** A primary "Sign in" button and social media login buttons for Google and Facebook.
     - **Footer:** A prompt to join if the user doesn’t have an account.
6. **Test the Application:**
   - Run the app using:
     ```sh
     npx expo start
     ```
   - Test on a physical device with the Expo Go app and ensure all components render as expected.

---
