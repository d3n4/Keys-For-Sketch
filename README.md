## Attention! Plugin Support Has Been Discontinued
Since I don't have much time for further plugin developement and new Sketch releases produce bugs pretty often I decided to discontinue the project support. Sorry.

Update: All sources are now available in this repo. Enjoy!

---

![](./Assets/img_cover.png)

<br />
<img src="https://d26dzxoao6i3hh.cloudfront.net/items/0z1f0k2Y0T182m343E1M/Group%202.svg" width="90" align="left">

# Keys For Sketch

<br />
Keys is a full-featured shortcut manager for Sketch. Integrated directly to Preferences window it helps you to customize shortcuts easily.
<br />
<br />

1. [Installation](#installation)
1. [Features](#features)
1. [Usage](#usage)
1. [FAQ](#faq)
1. [Support Project](#support-project)

## Installation
Keys installation is way the same as any other plugins. Just download latest release and double-click it.

[<img src="./Assets/btn_release.svg">](https://github.com/exevil/Keys-For-Sketch/releases/latest) [<img src="./Assets/btn_sketchpacks.svg">](https://sketchpacks.com/exevil/Keys-For-Sketch/install)

## Features
* Easily menu shortcuts customization
* Single-character shortcuts customization (like Pencil or Vector) 
* Shortcut conflicts resolving
* Any third-party plugins support
* Preferences window integration
* Intuitive lightning-fast UI
* Instant menu search
* Modern Sketch v45 plugin updating system support

## Usage
1. Open Sketch Preferences (⌘+,)
1. Select `Keys` tab
1. Choose menu item for shortcut redefinition
1. Click on its shortcut or on `...` on the right side
1. Press new short 
1. Resolve conflict if needed
1. Enjoy

## FAQ
#### — There is a Keys-related bug in latest beta version of Sketch. What should I do?
The only you can do is check [the issues list](https://github.com/exevil/Keys-For-Sketch/issues) and report your issue if no-one did it before. Right now Keys supports only the latest stable Sketch version, so you should expect an update right after its release.

#### — Where can I see the changelog?
On the [Releases](https://github.com/exevil/Keys-For-Sketch/releases) page.

#### — How to restore default Sketch shortcuts?
Use «Restore Default Shortcuts...» command from plugin menu. *It should remove any user shortcut data includinge one that defined directly in System Preferences.*

#### — How Keys will affect custom shortcuts I defined earlier in System Preferences?
Since Keys is using default system storage for shortcuts it shouldn't affect previously set shortcuts without additional user actions like «Restore Default Shortcuts...» command from plugin menu.

#### — Can't see my Keys shortcuts in System Preferences. Is it something wrong?
Since System Preferences caches shortcut values from storage once upon a startup you need to completely relaunch it to get updated shortcut data there.

#### — What happens with my custom shortcuts if I remove Keys?
Nothing, because all your shortcuts were defined in System Preferences.

#### — I removed Keys and my custom shortcuts manually from System Preferences, but tools with single-character shortcuts (like Pencil or Vector) are still using previously defined values. How to reset it to defaults too?
Since Sketch manages single character shortcuts by itself, you should delete `keyBindings.plist` from `~/Library/Application Support/com.bohemiancoding.sketch3/` folder and restart Sketch to return default tools shortcuts.

#### — Some menu items aren't shown in Keys. How to fix?
Internally Sketch may not properly draw some menu items prior to their first appearance in menu, that's why the only way to make these kind of menu items configurable with Keys is to manually access it through the app menu first.

#### — Keys conflicts with other plugins that using earlier Swift versions. Is there any way to fix it?
Unfortunately, there isn't. In simple terms, there's no capability between different Swift versions right now so it may produce an errors at runtime.

But it's not really a big deal. Firstly, the Swift team has already announced that ABI capability feature is planned for the next major Swift release and this is the first priority right now. Secondly, plugins can't conflict each other while the latest available Swift version is used for all of them and requesting author for an update may be a good temporary solution for this problem.

#### — Why I can't remove default shortcut from a menu item?
Since Keys plugin is wrapping a default System Preferences shortcut assignment flow it follows the same rules. So any default shortcut are constant until you either replace it with your own or use the same combination for another menu item.

#### — Why it's not possible to assign a single-character shortcut to menu item other than specific items under the insert menu?
Since Sketch itself is using an internal predefined list of menu items that allowed a single-character shortcut to be set, Keys can customize single-character shortcuts only for these items.

#### — My issue isn't listed here. What now?
Please check the [open issues list](https://github.com/exevil/Keys-For-Sketch/issues) and feel free to create a new one if you don't see your problem there.

## Support Project
I spent a lot of time to make this project real so any feedback or donation is really matters. It's wonderful to see that things you do are really making people's lives easier.

[<img src="./Assets/btn_support.svg">](https://www.paypal.me/exevil/10)

###### Please note that if you're sending your donation from Russian Federation only Russian Roubles will be accepted.
