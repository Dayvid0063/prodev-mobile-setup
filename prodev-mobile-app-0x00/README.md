# First Mobile App Setup

This documentation outlines the steps taken to create and scaffold a React Native app using the Expo Router template.

## Steps Followed

1. Navigated to the project directory:
   ```bash
   cd prodev-mobile-setup
   ```

2. Initialized a new Expo project using the Expo Router template:
   ```bash
   npx create-expo-app@latest prodev-mobile-app-0x00
   ```

3. Modified the home screen by editing `app/(tabs)/index.tsx`:
   - Changed the default text `Welcome!` to `** First App Created **`.

4. Ran the development server:
   ```bash
   npx expo start
   ```
   - Scanned the QR code using Expo Go on my device to test the app.

5. Reset the project using:
   ```bash
   npm run reset-project
   ```

## Observations from `reset-project`

- The `reset-project` command resets the project to its initial state, removing any changes made to the files.
- It reinitializes the project structure, which can be useful for debugging or starting fresh.
