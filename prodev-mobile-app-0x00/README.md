# Welcome to your Expo app 👋

This is an [Expo](https://expo.dev) project created with [`create-expo-app`](https://www.npmjs.com/package/create-expo-app).

## Get started

1. Install dependencies

   ```bash
   npm install
   ```

2. Start the app

   ```bash
   npx expo start
   ```

In the output, you'll find options to open the app in a

- [development build](https://docs.expo.dev/develop/development-builds/introduction/)
- [Android emulator](https://docs.expo.dev/workflow/android-studio-emulator/)
- [iOS simulator](https://docs.expo.dev/workflow/ios-simulator/)
- [Expo Go](https://expo.dev/go), a limited sandbox for trying out app development with Expo

You can start developing by editing the files inside the **app** directory. This project uses [file-based routing](https://docs.expo.dev/router/introduction).

## Get a fresh project

When you're ready, run:

```bash
npm run reset-project
```

This command will move the starter code to the **app-example** directory and create a blank **app** directory where you can start developing.

## Learn more

To learn more about developing your project with Expo, look at the following resources:

- [Expo documentation](https://docs.expo.dev/): Learn fundamentals, or go into advanced topics with our [guides](https://docs.expo.dev/guides).
- [Learn Expo tutorial](https://docs.expo.dev/tutorial/introduction/): Follow a step-by-step tutorial where you'll create a project that runs on Android, iOS, and the web.

## Join the community

Join our community of developers creating universal apps.

- [Expo on GitHub](https://github.com/expo/expo): View our open source platform and contribute.
- [Discord community](https://chat.expo.dev): Chat with Expo users and ask questions.

# Expo Router App Setup

## Steps Followed for Scaffolding

### **Navigating to the Project Directory**

```bash
cd prodev-mobile-setup
```

### **Initializing a New Expo Project**

```bash
npx create-expo-app@latest .
```

This command created a new React Native project using the Expo Router template.

The setup included folders such as /app, /components, /hooks, and /constants.

### **Modifying the Home Screen**

Opened the file:

```bash
app/(tabs)/index.tsx
```

Replaced the text Welcome! with:

**First App Created.**
Saved the file and observed automatic reloading in the Expo Go app.

### **Running and Testing the Application**

Started the development server using:

```bash
npx expo start --tunnel
```

The --tunnel flag was required for proper device connection since the normal command without it did not work.

Scanned the QR code using Expo Go on an Android device, and the app loaded successfully.

Verified that changes in the source code were reflected instantly (hot reload).

## **Observations from the reset-project Command**

Ran the reset command:

```bash
npm run reset-project
```

The terminal prompted:

Do you want to move existing files to /app-example instead of deleting them? (Y/n):
I entered n to skip moving files.

The following directories were deleted:

/app

/components

/hooks

/constants

/scripts

New files and structure were automatically recreated:

```bash
📁 New /app directory created
📄 app/index.tsx created
📄 app/_layout.tsx created
```

The console displayed:

```bash
✅ Project reset complete. Next steps:
1. Run `npx expo start` to start a development server.
2. Edit app/index.tsx to edit the main screen.
```

After running:

```bash
npx expo start --tunnel
```

The project restarted successfully.

The app opened correctly again in Expo Go.
