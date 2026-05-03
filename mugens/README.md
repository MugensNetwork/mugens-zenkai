## Next Steps

| Item | Required for... | How |
|---|---|---|
| `ascAppId` in `eas.json` | Submitting to the App Store | Create the app in App Store Connect first. |
| `GoogleService-Info.plist` | iOS push notifications | Firebase Console → add an iOS app with bundle ID `app.mugens.zenkai`. |
| Sentry | Production error tracking | Optional; skip for now. |
| Assets/icons | Branding | You already mentioned this will be handled later. |
| `primaryColor: '#006AFF'` | Splash screen color / Android adaptive icon color | Set this once the visual identity is defined. |
| `code-signing/certificate.pem` | Signed OTA updates | Only required if using EAS Update in production. |

EXPO_PUBLIC_SENTRY_DSN — Sentry
EXPO_PUBLIC_BLUESKY_PROXY_DID and EXPO_PUBLIC_CHAT_PROXY_DID — AppView/PDS at mugens.org

## Build and submit to the app stores
npx eas-cli@latest build --platform all --auto-submit