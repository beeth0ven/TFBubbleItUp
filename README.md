# TFBubbleItUp

[![CI Status](http://img.shields.io/travis/Ales Kocur/TFBubbleItUp.svg?style=flat)](https://travis-ci.org/Ales Kocur/TFBubbleItUp)
[![Version](https://img.shields.io/cocoapods/v/TFBubbleItUp.svg?style=flat)](http://cocoapods.org/pods/TFBubbleItUp)
[![License](https://img.shields.io/cocoapods/l/TFBubbleItUp.svg?style=flat)](http://cocoapods.org/pods/TFBubbleItUp)
[![Platform](https://img.shields.io/cocoapods/p/TFBubbleItUp.svg?style=flat)](http://cocoapods.org/pods/TFBubbleItUp)

![preview](https://raw.githubusercontent.com/thefuntasty/TFBubbleItUp/master/preview.gif)

## Usage

Just place UIView in your controller wherever you want and make it as TFBubbleItUpView subclass. It is configured as IBDesignable so it will show up. The content size is calculated by the view itself, no need to use height constraint. Just set in Interface builder Intrinsic size to placeholder - width check None and height choose what suit you best.

![Intrinsic size](https://github.com/thefuntasty/TFBubbleItUp/blob/master/intrinsic-size.png)

## Configuration

BubbleItUp is highly configurable. There is configuration file called *TFBubbleItUpViewConfiguration* with class variables for configuration.

```swift
/// Background color for cell in normal state
public static var viewBackgroundColor = UIColor(red: 0.918, green: 0.933, blue: 0.949, alpha: 1.00)
/// Background color for cell in edit state
public static var editBackgroundColor = UIColor.whiteColor()

/// Font for cell in normal state
public static var viewFont = UIFont.systemFontOfSize(12.0)

/// Font for cell in edit state
public static var editFont = UIFont.systemFontOfSize(12.0)

/// Font color for cell in view state
public static var viewFontColor = UIColor(red: 0.353, green: 0.388, blue: 0.431, alpha: 1.00)

/// Font color for cell in edit state
public static var editFontColor = UIColor(red: 0.510, green: 0.553, blue: 0.596, alpha: 1.00)

/// Corner radius for cell in view state
public static var viewCornerRadius: Float = 2.0

/// Corner radius for cell in edit state
public static var editCornerRadius: Float = 2.0

/// Height for item
public static var cellHeight: Float = 25.0

/// View insets
public static var inset: UIEdgeInsets = UIEdgeInsetsMake(5, 5, 5, 5)

/// Interitem spacing
public static var interitemSpacing: CGFloat = 5.0

/// Line spacing
public static var lineSpacing: CGFloat = 5.0

/// Keyboard type
public static var keyboardType: UIKeyboardType = UIKeyboardType.EmailAddress

/// Keyboard return key
public static var returnKey: UIReturnKeyType = UIReturnKeyType.Done

/// Field auto-capitalization type
public static var autoCapitalization: UITextAutocapitalizationType = UITextAutocapitalizationType.None

/// Field auto-correction type
public static var autoCorrection: UITextAutocorrectionType = UITextAutocorrectionType.No

/// If true it creates new item when user types whitespace
public static var skipOnWhitespace: Bool = true

/// If true it creates new item when user press the keyboards return key. Otherwise resigns first responder
public static var skipOnReturnKey: Bool = false
```

## Requirements

TFBubbleItUp uses Swift 2.0. Target deployment iOS 8.0 and higher.

## Installation

TFBubbleItUp is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod "TFBubbleItUp"
```

## Author

Ales Kocur, ales@thefuntasty.com

## License

TFBubbleItUp is available under the MIT license. See the LICENSE file for more info.
