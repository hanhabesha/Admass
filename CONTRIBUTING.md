## π Contribute

π Thanks for deciding to contribute to the project.

As of now, the project contains **OVER 10K LINES OF CODE**.

Recently, it is migrated to use [Provider](https://github.com/rrousselGit/provider) for its state management. At few, places `StatefulWidgets` are still present.

The project supports sorting of music based on media metadata tags & native playback directly from file explorer etc. The whole user interface strictly follows the material design guidelines.

Checkout [project structure](https://github.com/alexmercerind/harmonoid#-project) to get started. You may also join our [Discord Server](https://discord.gg/ZG7Pj9SREG). New Flutter developers are also welcomed.

The plan of project is to bring the best, cross platform music experience for all users. Fork the project today & add your features. We are actively looking for contributors. If you decide to contribute, add yourself to the about page of the app.

## π Project

Glad you're interested in contributing to the project, here is the project structure for guiding you to this codebase.

Labels marked with `*` have scope for improvement in future.

```
β   main.dart                     [Everyone knows this.]
β
ββββcore                          [Internal application logic.]
β       collection.dart           [For sorting, discovering, handling, updating, refreshing etc. of music.]
β       fileintent.dart           [For dealing with intents to open audio files.]
β       configuration.dart        [For saving application configuration.]*
β       discover.dart             [For interacting with server.]
β       download.dart             [For fetching content.]
β       mediatype.dart            [Various media structures used within application.]
β       playback.dart             [For playback using assets_audio_player or dart_vlc.]*
β
ββββinterface                     [Application user interface.]
β   β
β   ββββcollection                [Widgets & screens related to music collection.]
β   β
β   ββββsettings                  [Widgets & screens related to application settings.]
|
β   ββββdiscover                  [Widgets & screens related to music discovery.]
β   β
β   β   nowplaying.dart           [Now playing widgets & screen.]
β   β   harmonoid.dart            [Root Widget of application.]
β   β   home.dart                 [Child of Harmonoid widget, contains tabs for different screens.]
β   β   exception.dart            [A minimal MaterialApp to replace Harmonoid in case of any exception.]
β   β   changenotifiers.dart      [General ChangeNotifiers for state management.]
β
ββββutils
β       methods.dart              [General utility methods used across the application.]
β       widgets.dart              [Various Widgets that bring application to life.]
β
ββββconstants                     [General globalization related classes.]*
        language.dart
        strings.dart
```
