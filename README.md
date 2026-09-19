# Pulse

A small personal expense tracker, built to get hands-on again with the current React Native ecosystem. I've been away from RN for a while, and a lot has shifted — Expo as the default starting point, Expo Router instead of wiring up navigation by hand, EAS instead of local native builds. This project is my way of touching all of that end to end instead of just reading about it.

The app itself stays intentionally simple: log in, add an expense, see your transactions, done. The point isn't the expense tracker — it's everything underneath it.

## What's in it

- Email/password auth
- Add a transaction, optionally attach a photo of the receipt
- Transaction list that updates in real time
- A basic profile screen

## Stack

- [Expo](https://expo.dev) + [Expo Router](https://docs.expo.dev/router/introduction/) for file-based navigation
- Firebase — Auth, Firestore, security rules scoped per user
- Zustand for state
- react-hook-form + zod for forms and validation
- expo-camera / expo-image-picker for the receipt photo
- EAS for builds
- GitHub Actions for CI

## Status

Work in progress, built one piece at a time rather than scaffolded all at once.

## Running it

```bash
npm install
npx expo start
```

From there, open it in a simulator, an emulator, or Expo Go.
