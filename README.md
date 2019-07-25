# angular-ionic-recipe

https://www.youtube.com/watch?v=r2ga-iXS5i4


## Getting Start:

install npm ...  

- Create project, through \temp folder, if already having github project.

ionic start  

- ionic serve

## Building Project:

ng g c recipes  
ionic generate,

ionic generate page recipes/recipe-detail

## Build to Android and iOS

### Android

`ionic capacitor add android`

[error] Capacitor could not find the web assets directory "C:\Github\angular-ionic-recipe\www".  
--> Need to run `ng build` first to generate www folder.

Now you can run npx cap open android to launch Android Studio

- After any code change, do `ng build` and then run `ionic capacitor copy android`

- Or, just do `ionic capacitor run android`, `ionic capacitor run android -l` for live reload.

### iOS

- `xcode-select` to test if env ok, or `xcode-select --install` to install command line tools

- `ionic capacitor add ios`, "-" is not allowed in appId

- `ng build`, `ionic capacitor copy ios`

- `ionic capacitor run ios`, also open xcode. Make sure Signing with a team

- run on connected devices

- `ionic capacitor run ios -l`



