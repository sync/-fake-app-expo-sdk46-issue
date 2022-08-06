# fake-app

Sample reproduction app from expo SDK 46 iOS simualtor app install issue

# Reproduction

create a new project with: `npx create-expo-app --template expo-template-blank-typescript@sdk-46`

add dev client: `yarn expo install expo-dev-client`

then run: `yarn expo run:ios`

## expected

app to be installed and then launched into current iOS simulator

## actual

app is installed but never launched...

```
› Metro waiting on
com.sync.pluviae://expo-development-client/?url=http%3A%2F%2F192.168.4.52%3A8081
› Scan the QR code above with Expo Go (Android) or the Camera app (iOS)

› Press a │ open Android
› Press i │ open iOS simulator
› Press w │ open web

› Press r │ reload app
› Press m │ toggle menu

› Press ? │ show all commands

› Installing on iPhone 13 mini
```

If I follow those exact same steps using the SDK 45, the app get installed and then launched inside my current iOS simulator.
