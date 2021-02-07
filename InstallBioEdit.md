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
  <img src="https://github.com/adeslatt/BioEditMultiSequenceAlignment/blob/master/assets/BrewInstallWineStableOnMac.png"  width="750" align="left" >
</p>
<br/><br/>

Now that wine is installed, change to a directory where you will install windows programs -- 
TODO:  Make a container for this program

For me, to keep organized, I have my work organized by year and projects including where I have checked out programs I want to use, are organized under year and project.  I also have my laptop synchronized back up with dropbox - so that the files are not always on my desktop but come in when I need them.

I do this through my consultancy and I am set up as a user under there.

```bash
cd Scitechcon
cd Anne\ DeslattesMays
cd 2021
cd 2021Projects
cd WindowsPrograms
cd bioedit
```

The file was downloaded from [SoftwareInformer](https://bioedit.software.informer.com/7.2/)
which downloaded a `bioedit.zip` file to Downloads which I moved into the bioedit directory.

Taking a look of the contents of the directory after moving the file and unzipping

```bash
 mv ~/Downloads/bioedit.zip .
 unzip bioedit.zip
```
Still was not working so I did the following
1. Installed Xcode
2. Updated XQuartz

Had to reboot for the XQuarts to become the default X11

