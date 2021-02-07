# Platform Specific Installs for using BioEdit to do Multiple Sequence Alignment

## Mac Install 

First step install homebrew

```Bash
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Then you need to run brew doctor
```Bash
brew doctor
```

If you need to agree to Xcode license -- you can do that by running
```Bash
sudo xcodebuild -license
```

[Installing Wine on Mac](https://www.davidbaumgold.com/tutorials/wine-mac/)

On my mac, I have already brew installed
```Bash
brew cask install wine-stable
```

This caused an error -- I had to install cask

```Bash
brew install cask
```

This still caused an error -- so instead I just ran
```Bash
brew install wine-stable
```
which on my screen outputs the following image
<p align="center">
  <img src="https://github.com/adeslatt/BioEditMultiSequenceAlignment/blob/master/assets/BrewInstallWineStableOnMac.png"  width="500" align="center" >
</p>
<br/><br/>
