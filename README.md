# `🌩 Ionic-base` 

### SETUP
##### clone
```sh
git@github.com:leocastroz/ionic-base.git
```

##### install
```sh
npm install
```

##### preview
```sh
npm run dev
```
```sh
ionic serve
```
<br>
<br>

### Generating Android
##### step-1
```sh
ionic cap sync
```

##### step-2
```sh
ionic cap build android --no-open cd android
```

#### `cap` = capacitor
#### `--no-open` = won't open androidStudio

##### step-3
```sh
cd android
```

<br>
<br>

⚠️ When creating the 'Android' folder you should add this line to your project in the`gradle.properties`:
```sh
android.overridePathCheck=true
```

<br>
<br>

#### step-4
```sh
./gradlew assembleDebug
```

##### `assembleDebug` = to use it you don't need an Android authenticated key

```sh
./gradlew bundleRelease
```
```sh
./gradlew assembleRelease
```

##### `assembleRelease` = an authenticated Android key is required
