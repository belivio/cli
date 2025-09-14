# Upgrading Your App to Expo SDK 54 (from 53)

Follow these steps to upgrade your app safely and cleanly:

---

## 1. Update to the Latest Version of EAS CLI (if you use it)

```sh
npm i -g eas-cli
```

---

## 2. Upgrade All Dependencies to Match SDK 54

```sh
npx expo install expo@^54.0.0 --fix
```

---

## 3. Check Resolutions/Overrides in `package.json`

- Verify that any **resolutions** or **overrides** you have are still needed.
- Example: Remove `metro` and `metro-resolver` overrides if you added them for `expo-router` in a previous SDK release.
- If you configured `metro.config.js` for a monorepo setup, review the updated [Work with monorepos guide](https://docs.expo.dev/guides/monorepos/) to see if changes are necessary.

---

## 4. Run Expo Doctor to Catch Known Issues

```sh
npx expo-doctor@latest
```



