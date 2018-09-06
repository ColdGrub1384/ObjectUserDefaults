# ObjectUserDefaults

An object oriented `UserDefaults`.

`UserDefaults` uses methods to get values and set values with given keys, but you have to pass keys as parameters each time you want to set or get a value. With `ObjectUserDefaults`, each item in stored in `UserDefaults` is represented by an object and its value can be set and gotten trough that. That's mean that instead of storing keys in constant, you can store direct references to items.

## Usage

```swift
import ObjectUserDefaults

let item = ObjectUserDefaults.standard.item(forKey: "Key") // Creates a reference to the key "Key"

print(item.value) // Prints the value of the key
item.value = true // Sets the value of the key
print(item.boolValue) // Prints the boolean value of the key
```

## Installation

### Cocoapods

`pod 'ObjectUserDefaults'`

### Manual

Copy this repo to yours or add it as submodule, drag the xcode project to your one and embed the framework in your target's info tab.

## Documentation

See the docs [here](https://coldgrub1384.github.io/ObjectUserDefaults)
