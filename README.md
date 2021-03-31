# flutter_tab_indicator_styler

[![Pub](https://img.shields.io/pub/v/flutter_tab_indicator_styler.svg)](https://pub.dartlang.org/packages/flutter_tab_indicator_styler)
[![Awesome Flutter](https://img.shields.io/badge/Awesome-Flutter-blue.svg?longCache=true&style=flat-square)]()
[![Awesome Flutter](https://img.shields.io/badge/Platform-Android_iOS-blue.svg?longCache=true&style=flat-square)]()
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](/LICENSE)

<p align="center">
  <img width="460"  src="https://raw.githubusercontent.com/flutter-fast-kit/tab_indicator_styler/master/images/tab_styler_logo.png">
</p>

Add beautiful and trending tab indicators directly to your default Flutter TabBar.

## Features 💚

- Supports Android, iOS, Web
- Can be directly added to the default TabBar
- 3 different styles of TabIndicator
- Highly customizable

## Demo

<p align="center">
  <img src="https://raw.githubusercontent.com/flutter-fast-kit/tab_indicator_styler/master/images/demo.gif" height="480"> 
</p>

## Styles

#### DotIndicator

```Dart
 /// Radius of the dot
  final double radius;

  /// Color of the dot
  final Color color;

  /// Distance from the center, if you the value is positive, the dot will be positioned below the tab's center
  /// if the value is negative, then dot will be positioned above the tab's center
  final double distanceFromCenter;

  /// [PagingStyle] determines if the indicator should be fill or stroke
  final PaintingStyle paintingStyle;

  /// StrokeWidth, used for [PaintingStyle.stroke]
  final double strokeWidth;

```

### MaterialIndicator

```Dart
  /// Height of the indicator. Defaults to 4
  final double height;

  /// Determines to location of the tab, [TabPosition.bottom] set to default.
  final TabPosition tabPosition;

  /// topRight radius of the indicator, default to 5.
  final double topRightRadius;

  /// topLeft radius of the indicator, default to 5.
  final double topLeftRadius;

  /// bottomRight radius of the indicator, default to 0.
  final double bottomRightRadius;

  /// bottomLeft radius of the indicator, default to 0
  final double bottomLeftRadius;

  /// Color of the indicator, default set to [Colors.black]
  final Color color;

  /// Horizontal padding of the indicator, default set 0
  final double horizontalPadding;

  /// [PagingStyle] determines if the indicator should be fill or stroke, default to fill
  final PaintingStyle paintingStyle;

  /// StrokeWidth, used for [PaintingStyle.stroke], default set to 2
  final double strokeWidth;
```

#### RectangularIndicator

```Dart
/// topRight radius of the indicator, default to 5.
  final double topRightRadius;

  /// topLeft radius of the indicator, default to 5.
  final double topLeftRadius;

  /// bottomRight radius of the indicator, default to 0.
  final double bottomRightRadius;

  /// bottomLeft radius of the indicator, default to 0
  final double bottomLeftRadius;

  /// Color of the indicator, default set to [Colors.black]
  final Color color;

  /// Horizontal padding of the indicator, default set to 0
  final double horizontalPadding;

  /// Vertical padding of the indicator, default set to 0
  final double verticalPadding;

  /// [PagingStyle] determines if the indicator should be fill or stroke, default to fill
  final PaintingStyle paintingStyle;

  /// StrokeWidth, used for [PaintingStyle.stroke], default set to 0
  final double strokeWidth;

```

## How to use

```Dart
// Directly use inside yoru [TabBar]
TabBar(
  indicatorColor: Colors.green,
  tabs: [
    Tab(
      text: "Home",
    ),
    Tab(
      text: "Work",
    ),
    Tab(
      text: "Play",
    ),
  ],
  labelColor: Colors.black,
  // add it here
  indicator: DotIndicator(
    color: Colors.black,
    distanceFromCenter: 16,
    radius: 3,
    paintingStyle: PaintingStyle.fill,
  ),
),
```
