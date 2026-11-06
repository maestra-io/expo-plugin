# Maestra SDK for React Native Expo

The Maestra SDK allows developers to integrate mobile push notifications, in-app messages, and client events into your React Native Expo projects.

## Getting Started

These instructions will help you integrate the Maestra SDK into your React Native Expo app.

See the [React Native Expo integration guide](https://developers.maestra.io/docs/2133) for the full setup.

## Example app

`examples/MindboxExpoExample` is a sample app. Before you build it, set your own values:

- `endpointId` in `src/screens/HomeScreen.tsx`: replace the `YourProject.IosExpo` and `YourProject.AndroidExpo` placeholders with the iOS and Android endpoints of your Maestra project.
- `ios.bundleIdentifier` and `android.package` in `app.json` (`io.maestra.example.expo`): use your own application identifiers. Put a `google-services.json` that matches the Android package into `credentials/`.
- EAS project: run `eas init` to link the app to your Expo account. It writes `extra.eas.projectId` to `app.json`, which the app needs to get a push token.
- Apple team: set `ios.appleTeamId` in `app.json` (or the plugin's `iosDevTeam` option) to your Apple Developer team ID.
