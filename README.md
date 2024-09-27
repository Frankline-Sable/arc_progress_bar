## Arc Progress Bar

The Arc Progress Bar is an open source Flutter package that simplifies the creation of a curved or arc-shaped progress
bar widget. It offers a wide range of customization options for users, taking care of the intricate curve calculations
and animations on your behalf.

## Add Dependency

Add this to your pubspec.yaml dependencies:

```yaml
dependencies:
  arc_progress_bar_new: ^1.0.4
```

## How to use

First of all make sure to call the import

```dart
import 'package:arc_progress_bar_new/arc_progress_bar_new.dart';
```


Then just customize the widget's parameters.

```dart
  ArcProgressBar(
    percentage: _progressPercentage,
    arcThickness: 5,
    innerPadding: 16,
    animateFromLastPercent: true,
    handleSize: 10,
    backgroundColor: Colors.black12,
    foregroundColor: Colors.black
    )
```

<img src="https://raw.githubusercontent.com/Frankline-Sable/arc_progress_bar/main/example/screenshots/1.png" alt="Colored Nodes & Outlines" width="500"/>

---

## Screenshots & Implementations

### Example 1 - With custom Colors and Handle

<img src="https://raw.githubusercontent.com/Frankline-Sable/arc_progress_bar/main/example/screenshots/2.png" alt="With custom colors and handle" width="300"/>

```dart
 ArcProgressBar(
    percentage: _progressPercentage,
    arcThickness: 15,
    innerPadding: 48,
    strokeCap: StrokeCap.round,
    handleSize: 50,
    handleWidget: Container(
      decoration: const BoxDecoration(color: Colors.red)),
    foregroundColor: Colors.redAccent,
    backgroundColor: Colors.red.shade100,   
 ),
```

<br>

### Example 2 - With Icon And Texts

<img src="https://raw.githubusercontent.com/Frankline-Sable/arc_progress_bar/main/example/screenshots/3.png" alt="With Icons And Texts" width="300"/>

```dart
 ArcProgressBar(
    percentage: _progressPercentage,
    bottomLeftWidget: const Text("Level 3"),
    bottomRightWidget: const Text("240/300"),
    bottomCenterWidget: const Text("RECRUIT"),
    centerWidget: Image.asset("assets/images/insignia.png",
        height: 200, width: 200, fit: BoxFit.contain)),   
 ),
```

<br>

### Example 3 - Very Simple & Customizable

<img src="https://raw.githubusercontent.com/Frankline-Sable/arc_progress_bar/main/example/screenshots/4.png" alt="Very Customizable" width="300"/>

```dart
 ArcProgressBar(
   percentage: _progressPercentage,
   arcThickness: 5,
   innerPadding: 16,
   animateFromLastPercent: true,
   handleSize: 10,
   backgroundColor: Colors.black12,
   foregroundColor: Colors.black),
```

<br>


Very customizable, feel free to customize however you like! 😎
