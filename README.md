# SignApp
SignApp is a simple, minimal footprint script that will extract an IPA and repack it into a deb made for installing on an Apple TV or iOS device respectively.

## How does it work?
SignApp extracts an IPA, takes needed info from the info.plist to create a specialized control file, adds entitlements to the main binary and frameworks (so the app can be ran as root), then repacks it back into an ipa

## Instructions
1. Download the latest Installer from the releases page.
2. Simply double click the Installer, type your password when prompted, and let the script install SignApp and its dependencies.
3. Run SignApp [/path/to/ipa] to repack your IPA.

## Installer Info
The Installer script will automatically check for all dependancies and install them if needed using the package manager you currently have installed (Homebrew or MacPorts). If you do not have a package manager installed, it will install Homebrew and then the dependancies.

## Updating
Simply rerun the Installer script. It automatically pulls the latest SignApp from Github and installs it
