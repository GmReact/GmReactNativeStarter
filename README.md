# GmReactStarter Prerequisites

Install HomeBrew to machine
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
  
# Update HomeBrew to latest version
brew doctor
brew update

# Install React Native Dependencies and Build Tools
# Install Node.js
brew install node
  
# Install Watchman
brew install watchman

# Install XCode Command Line Tools
# Install apple select
xcode-select --install
  
# Install applesimutils
brew tap wix/brew
brew install wix/brew/applesimutils

# Android Setup
# Install Java
Download and install the latest Java SE Development Kit 8.

#Add Java home to your profile
echo 'export JAVA_HOME="$(/usr/libexec/java_home -v 1.8)"' >> ~/.profile

#Install Android Studio and NDK
# Install Android Studio
brew cask install android-studio
  
# Install Android NDK
brew cask install android-ndk
  
# Add ANDROID_NDK_HOME to your profile
echo 'export ANDROID_NDK_HOME="/usr/local/share/android-ndk"' >> ~/.profile

#Install the app on iOS
npm react-native run-ios

If any issues with cocoapods run the below command
sudo gem install cocoapods

and run pod install inside ios folder.

For more Debugging or machine setup please refer 
https://reactnative.dev/docs/environment-setup
