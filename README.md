![Twinkle](https://raw.github.com/piemonte/twinkle/master/twinkle.gif)

## Twinkle :sparkles:

`Twinkle` is a [Swift](https://developer.apple.com/swift/) and easy way to make any UIView in your iOS or tvOS app twinkle.

This library creates several CAEmitterLayers and animates them generating a sparkle effect.

[![Pod Version](https://img.shields.io/cocoapods/v/Twinkle.svg?style=flat)](http://cocoadocs.org/docsets/Twinkle/)
[![Build Status](https://travis-ci.org/piemonte/Twinkle.svg?branch=master)](https://travis-ci.org/piemonte/Twinkle)

# Quick Start

`Twinkle` is available and recommended for installation using the Cocoa dependency manager [CocoaPods](http://cocoapods.org/). You can also simply copy the `Twinkle.swift` file into your Xcode project.

## Xcode 8 & Swift 3

```ruby
# CocoaPods
pod "Twinkle", "~> 0.2.0"

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['SWIFT_VERSION'] = '3.0'
    end
  end
end

# Carthage
github "piemonte/Twinkle" ~> 0.2.0

# SwiftPM
let package = Package(
    dependencies: [
        .Package(url: "https://github.com/piemonte/Twinkle", majorVersion: 0)
    ]
)
```

## Xcode 8 & Swift 2.3 or Xcode 7

```ruby
# CocoaPods
pod "Twinkle", "~> 0.1.1"

# Carthage
github "piemonte/Twinkle" ~> 0.1.1
```

## Usage

The sample project provides an example of how to integrate `Twinkle`, otherwise you can follow this example.

``` Swift
   import Twinkle
```

``` Swift
   let view: UIView = UIView(frame: CGRect(x: 0, y: 0, width: 150, height: 50))
   self.view.addSubview(view)
   view.twinkle()
```

## Community

- Found a bug? Open an [issue](https://github.com/piemonte/twinkle/issues).
- Feature idea? Open an [issue](https://github.com/piemonte/twinkle/issues).
- Want to contribute? Submit a [pull request](https://github.com/piemonte/twinkle/pulls).

## Resources

* [Core Animation Reference Collection](https://developer.apple.com/library/ios/documentation/Cocoa/Reference/CoreAnimation_framework/index.html)
* [Shimmer](https://github.com/facebook/shimmer)
* [Swift Evolution](https://github.com/apple/swift-evolution)

## License

Twinkle is available under the MIT license, see the [LICENSE](https://github.com/piemonte/twinkle/blob/master/LICENSE) file for more information.
