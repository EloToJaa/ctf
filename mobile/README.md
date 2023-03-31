# Mobile exploitation

## Links

- [HackTricks](https://book.hacktricks.xyz/mobile-pentesting/android-app-pentesting)
- [Android Studio](https://developer.android.com/studio)
- [jadx](https://github.com/skylot/jadx)
- [Frida](https://frida.re/)

## Decompile apk

```sh
apktool d -r -s application.apk
```

## Compile apk

```sh
apktool b -f -d application
```

## Generate apk key

```sh
keytool -genkey -v -keystore my-release-key.keystore -alias alias_name -keyalg RSA -keysize 2048 -validity 10000
```

## Sign apk

```sh
jarsigner -verbose -sigalg SHA1withRSA -digestalg SHA1 -keystore my-release-key.keystore my_application.apk alias_name
```

## Verify apk

```sh
jarsigner -verify -verbose -certs my_application.apk
```

## React Native decompiler

```sh
npx react-native-decompiler -i index.android.bundle -o output
```
