# CH Products Joystick Map for Elite: Dangerous

Joystick maps and game configuration files for the [CH Products][]
[Fighterstick][] and [Pro Throttle][] HOTAS in [Elite: Dangerous][].

## About

This map is my own personal configuration that I've put together while playing
Elite: Dangerous. It has undergone a number of changes since the original
release reflecting both improvements in the layout, and changes introduced by
the game. The maps are presented here for others to use, either verbatim, or as
a base for a customised map.

### Version

This version of the map is designed for use with Elite: Dangerous 3.3 and above.

### Previous versions

Previous versions of the joystick maps, including the relevant README.md and
layout guides, can be found [here][previous]. Major version number changes
indicate complete overhauls of the map.

## Requirements

* [CH Products][] [Fighterstick][]
* [CH Products][] [Pro Throttle][]
* [CH Products][] [Control Manager][] software
* [Elite: Dangerous][] 3.3 or above
* Optional: PDF viewer

## Installation

Download and extract the [zip file][] containing the game files.

### Joystick Maps

Navigate to `Documents` and create a folder called `CH Control Manager` if it
does not already exist. Under that create a folder called `Maps` if it does not
already exist.

Within the extracted zip file under the `maps` folder you'll find two files. 
These need to be copied to the `CH Control Manager/Maps` folder.

![The load dialog](images/load.png)

Plugin your [Fighterstick][] and [Pro Throttle][], then launch the [CH Control
Manager][Control Manager]. Load `ed.map`. The load dialog should default to the
folder you copied your maps to. If it does not just navigate to that folder.

![The Download Button](images/download.png)

Once loaded click the `Download` button to enable the map.

### Game Configuration

Within the extracted zip file under the `config` folder you'll find two files
called `Custom.3.0.binds` and `StartPreset.start`. Copy these to
`%LOCALAPPDATA%\Frontier Developments\Elite Dangerous\Options\Bindings\`. Note:
`%LOCALAPPDATA%` points to the hidden `AppData\Local` folder for _your_ Windows
account. For example: `C:\Users\Dom\AppData\Local`.

## Layout Guide 

Within the extracted zip file, under the `guide` directory, you'll find the PDF 
guide containing the key bindings, and layout used by this map.

## Head-Look and UI Panels

I now play ED exclusively in VR so the mappings for head-look have been dropped
as I have no requirement for them. Similarly the settings for the various panels
are designed for playing in VR and may need tweaking in game (`Settings`,
`Controls`, find the section called `Mode Switches`, check `Enable UI Camera
Lock On`).

## Adding Rudder Pedals

I no longer own the CH Products [Pro Pedals][], however, I have had experience 
using them. You can add them to these maps by clicking the `Add Device` button 
and selecting the pedals from the list. 

## About The Author

This was all put together by [Cmdr Davis][]. I do the odd [YouTube][] video 
relating to [Elite: Dangerous][]. If you see me in game, say "Hi".

## Misc

The stick and throttle images used in the layout guide were commissioned by me.
Feel free to use and edit them for _personal_ use. If you're going to publish
the result please link back to this repository. You'll need to contact me if you
want to use the images commercially.

The map has been completely rebuilt to exclusively use keyboard presses rather
than button presses to allow for easier integration with [Voice Attack][].

Multi-crew and Fighter orders haven't been tested as yet as I don't have access
to either.

For some reason in DSS mode the game won't let you use the standard panel binds,
even though they don't do anything. As a result exit DSS requires the shift 
(pinky) button on the stick to be pressed along with the hat button.

## Caveat Emptor

With the exception of the PDF all the files contained in this project are text 
files so, in theory, nothing bad can happen to your system. That said, you're 
messing about with game config files so if you break anything, you get to keep 
both halves. If in doubt always back up.

[previous]: https://github.com/domdavis/ch-products-elite-map/releases/
[CH Products]: http://www.chproducts.com/
[Fighterstick]: http://www.chproducts.com/Fighterstick-v13-d-722.html
[Pro Throttle]: http://www.chproducts.com/Pro-Throttle-v13-d-719.html
[Elite: Dangerous]: http://www.elitedangerous.com/
[zip file]: https://github.com/domdavis/ch-products-elite-map/archive/master.zip
[Control Manager]: http://www.ch-hangar.com/forum/index.php/files/file/49-control-manager/
[Pro Pedals]: http://www.chproducts.com/Pro-Pedals-v13-d-716.html
[Cmdr Davis]: https://twitter.com/cmdr_davis 
[YouTube]: https://www.youtube.com/user/idomdavis
[Voice Attack]: https://voiceattack.com
