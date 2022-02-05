# AppleScript Askpass

![The prompt](https://user-images.githubusercontent.com/420820/152660505-6b444ae0-33f4-44a3-8337-ae2a832a4f09.png)
![The prompt when an incorrect password is entered](https://user-images.githubusercontent.com/420820/152660546-b318b1ba-0624-4b01-93bf-5e585e1b2453.png)

A pure AppleScript askpass (used to prompt the user for their sudo password).

For example, this could be used to run the Homebrew installer in an otherwise unattended manner:
```shell-script
SUDO_ASKPASS=applescript_askpass CI=true /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
