monkey.sublime
==============

This bundle lets you to use the multi-platform editor [Sublime Text](http://www.sublimetext.com) as an IDE for the [monkey programming language](http://www.monkeycoder.co.nz). It is based on [monkey.tmbundle](https://github.com/gingerbeardman/monkey.tmbundle).

Created by Matt Sephton, [http://www.gingerbeardman.com/monkey/](http://www.gingerbeardman.com/monkey/)

## Features

**Syntax Highlighting**  
Easily see keywords, constants, strings, comments, numbers and functions/classes/methods in your code

**Auto Completion of Keywords**  
Press the Tab key to expand to the first match after typing part of a keyword, Option+Escape will present a list of matches for you to choose from

**Expand Keywords into Code**  
Press the Tab key to expand one keyword into one or more lines of code, subsequent presses of tab intelligently jump you through the resulting code allowing you to fill in multiple parameters with minimal key strokes

**Build Systems**  
Quick and easy build by pressing ⌘B, current build system can be set in the Tools menu

**Easy Source Navigation**  
Navigate around your source using the index of functions, classes and methods

...and more to come

## Mac OS X

### Installation

Please check that the download is named `monkey.sublime` and not something else. You may have to rename it.

Unzip to:

	~/Library/Application Support/Sublime Text/Packages/

Next, you will need to add your monkey/bin folder to your system wide path. This is currently a bit awkward but will hopefully become easier as Sublime Text continues to be improved.

### Path
You will first need to confirm your monkey/bin location is in your shell path:

    echo "export PATH=\$PATH:/user/folder/monkey/bin" >> ~/.profile

Next, add the shell path to the system-wide environment:

    defaults write ${HOME}/.MacOSX/environment PATH "${PATH}"

Alternatively, you can manually edit `~/.MacOSX/environment.plist` or use the  [RCEnvironment](http://www.rubicode.com/Software/RCEnvironment/) preference pane. Either way, the goal is to add your monkey/bin path to the PATH variable in your environment.

You will need to restart for the changes to take effect.

## Windows

Support for Microsoft Windows is present. You will need to add your monkey/bin folder to the system PATH.

## Linux

There is currently no Linux support as Monkey does not currently support it.

## Support
You can talk about the bundle on the [official monkey forum](http://www.monkeycoder.co.nz/Community/posts.php?topic=593)

## Requirements
- Sublime Text 2 [http://www.sublimetext.com/2](http://www.sublimetext.com/2)
- monkey [http://www.monkeycoder.co.nz](http://www.monkeycoder.co.nz)

## License
monkey.sublime is made available under a [Creative Commons Attribution-Share Alike 3.0 Unported License](http://creativecommons.org/licenses/by-sa/3.0).

## Changelog

2011-10-08  
- Added FirstNode, LastNode, NextNode, PrevNode, Exp (v45c)  
- Added DisableKeyboard, EnableKeyboard (v45)  
- Added ACosr, ASinr, ATan2r, ATanr, Cosr, Sinr, Tanr (v44)  
- Added DrawPoly (v43)  
- Added App: UpdateRate  
- Added Audio: music commands (v35), Discard  
- Added Graphics: DeviceHeight, DeviceWidth, Frames, HandleX, HandleY, Height, Width  
- Added Lang: Print, Length, Resize, Compare, ToLower, ToUpper, Trim  
- Added List: Backwards, Clear, Count, First, IsEmpty, Last, LastNode, ObjectEnumerator, RemoveFirst, RemoveLast, Value, ToArray  
- Added Map: Set, Values, Key  
- Added Random: Seed  
- Added Set: Insert  
- Added Stack: Insert, Pop, Push, Top  

**2011-08-11**  
- Added LANG const  

**2011-08-09**  
- Removed extraneous JOY constants  
- Added missing JoyX/Y/Z keywords  
- Added TARGET const  
- Removed binary integer grammar which was resulting in incorrect display of numerical values  

**2011-08-08**  
- Updated language definition to the latest one from monkey.tmbundle, lots of changes:  
- Added else/elseif snippet  
- Reduced number of foldable elements  
- Added keyEquivalent ^⌥⇧+M to activate bundle  
- Renamed bundle from monkey to Monkey  
- Removed preprocessor grammar  
- Removed framework grammar  
- Removed module grammar  
- Added better if/then/elseif/else/endif handling  
- Added bitwise complement operator  
- Removed superstrict reference  
- Tidied block comment grammar  
- Replaced instances of (?:(?:^|;)\s*) with neater \b (regexp boundary)  
- Removed references to integer number symbol %  
- Corrected PI constants regexp  
- Removed pointerops grammar  
- Removed unused types from types grammar  
  
**2011-06-01**  
- Added one build system per target, should default to HTML5 but may need specifying manually  
  
**2011-05-31**  
- Updated language definition to the latest one from monkey.tmbundle (v40)  
  
**2011-05-19**  
- Updated language definition to the latest one from monkey.tmbundle (v39)  
  
**2011-04-20**  
- Added workaround for path issue  
- Added installation notes  
- Fixes for some broken snippets  
- Added file_regex so errors can be located  
  
**2011-04-19**  
- Added multiple command line parameters, thanks to Adam Woodall  
  
**2011-04-18**  
- Added build system (path to trans needs to be hard coded - you will have to edit the Monkey.sublime-build file)  
  
**2011-04-08**  
- Initial release  

## To do

- support for tab [completions](http://sublimetext.info/docs/extensibility/completions.html)  
- support for context sensitive help through a [command](http://sublimetext.info/docs/extensibility/plugins.html#types-of-commands)  

