# iPwnStrap

A full featured bootstrap for iOS 15.0-17.0 A8-A17 & M1+M2 using roothide.

##### *WARNING:* By using this software, you take full responsibility for what you do with it. Any unofficial modifications to your device may cause irreparable damage. Refer to the FAQ linked in the `Usage` section for safe usage of this software.

iPwnStrap is available to download on this repositories [Releases](https://github.com/BananeRapeuse/iPhoneBeenPwned/releases).

## Building

If you do not have access to MacOS, refer to the FAQ in the `Usage` section to build with GitHub Actions instead.

You'll need MacOS to build, as you require Xcode from the App Store. Simply having Xcode Command Line Tools is *insufficient*. Here's how to build the Bootstrap:

 1. Update/Install Theos with roothide support
    
    ```
    bash -c "$(curl -fsSL https://raw.githubusercontent.com/roothide/theos/master/bin/install-theos)"
    ```
    *If you encounter errors from a previous Theos installation, remove Theos in its entirety before continuing.*

 2. Clone the GitHub repository and enter directory

    ```
    git clone https://github.com/BananeRapeuse/iPwnStrap/ && cd Bootstrap
    ```

 3. Build `Bootstrap.tipa`

    ```
    make package
    ```

 4. Transfer `Bootstrap.tipa` from `./packages/` to your device and install it with TrollStore

## Usage

The iPwnStrap application **must** be installed with [TrollStore](https://ios.cfw.guide/installing-trollstore/). Use version `2.0.9` or later for enabling developer mode on-device.

Tweaks not compiled or converted to roothide will not work out-of-the-box with Pwnstrap. Refer to the FAQ below on how to use roothide Patcher.

By design, the app does not inject tweaks into any applications by default. To enable tweak injection into an application, press `App List` in the app, and enable the toggle of the application you want to inject into. Injection into `com.apple.springboard` or daemons is not possible with the iPwnStrap. Refer to the FAQ below on injection into `com.apple.springboard`.

**A FAQ** is available [here](https://github.com/dleovl/Bootstrap/blob/faq/README.md). (roothide Bootstrap faq)

## Develop tweaks

Both rootful and rootless tweaks aren't out-of-the-box compatible with roothide, so you'll need to develop them specifically to support it. You can refer to the developer documentation [here](https://github.com/roothide/Developer).

## The "Our Table" Icon

The ProcursusTeam logo was originally made by [@TheAlphaStream](https://github.com/TheAlphaStream), and later edited by [@sourcelocation](https://github.com/sourcelocation).

