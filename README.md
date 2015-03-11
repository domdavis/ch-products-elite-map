# CH Products Joystick Map for Elite: Dangerous

Joystick maps and game configuration files for the [CH Products][] [Fighterstick][] and [Pro Throttle][] HOTAS in [Elite: Dangerous][].

## About

These maps are my own personal configuration that I've put together while playing Elite: Dangerous. The maps have evolved over time and are presented here as it's a much easier way of distributing changes. As the game evolves and my play style evolves you may see additional changes. Feel free to download, use and tweak for your own setup.

## Requirements

* [CH Products][] [Fighterstick][]
* [CH Products][] [Pro Throttle][]
* [CH Products][] [Control Manager][] software
* [Elite: Dangerous][] 1.2 or above
* Optional: PDF viewer

## Installation

Download and extract the [zip file][] containing the game files.

### Version

This version of the map is designed for use with Elite: Dangerous 1.2 and above.

### Previous versions

Previous versions of the joystick maps, including the relevant README.md, can 
be found [here][previous]

### Joystick Maps

Navigate to `My Documents` and create a folder called `CH Control Manager` if it doesn't already exist.

Within the extracted zip file under the `maps` folder you'll find two files
called `elite.cms` and `elite.map`. These need to be copied to the `CH Control Manager` folder.

Plugin your [Fighterstick][] and [Pro Throttle][], then launch the [CH Control Manager][Control Manager] and load the `elite.map`. The load dialog should default to the folder you copied your maps to. If it doesn't just navigate to that folder. Once loaded click the `Download` button to enable the map.

### Game Configuration

Within the extracted zip file under the `config` folder you'll find two files called `Custom.binds` and `StartPreset.start`. Copy `Custom.binds` to
`C:\Users\USER\AppData\Local\Frontier Developments\Elite Dangerous\Options\Bindings\Custom.binds`. Change `USER` to be your username. `AppData` is a hidden folder so you’ll need to enable _Show Hidden Files_ to see it.

You can optionally copy `StartPreset.start` to the same folder. All this does is tell the game to use the custom bindings by default. If you don't copy the file you'll need select the custom layout from within the game under the input settings.

## Cheat Sheet

Within the root of the extracted zip file you'll find a file called `layout.pdf`. This file contains the button layout for the joystick map which can be used as a cheat sheet.

## Axis Layout

### Fighterstick

Axis                                 | Action
------------------------------------ | ------
`Stick Forward`                      | Pitch down
`Stick Back`                         | Pitch up
`Stick Left`                         | Roll left
`Stick Right`                        | Roll right
`Throttle Wheel` forward<sup>1</sup> | Enable `Throttle`
`Throttle Wheel` back<sup>1</sup>    | Disable `Throttle`

> <sup>1</sup> The throttle wheel on the stick is used to enable and disable analogue throttle inputs from the [Pro Throttle][]. This allows you to bring the ship to a full stop even if your throttle is suffering from drift and not returning completely to zero when fully back. With the wheel moved back input from the [Pro Throttle][] is ignored and a throttle setting of zero (full stop) is used. With the wheen moved forward the [Pro Throttle][] is enabled. You should ensure the throttle wheel is fully forward if the [Pro Throttle][] is not responding.  

### Pro Throttle

Axis                     | Action
------------------------ | ------
`Throttle` fully back    | 0% Throttle
`Throttle` fully forward | 100% Throttle
`Thumb Stick` up         | Thrust up
`Thumb Stick` down       | Thrust down
`Thumb Stick` left       | Thrust left
`Thumb stick` right      | Thrust right

**Note:** Analogue inputs for reverse thrust (0% to -100%) are achieved by holding the `back` button on the front 4-way hat on the throttle. With this button held the mappings for the throttle axis become

Axis                     | Action
------------------------ | ------
`Throttle` fully back    | 0% Throttle
`Throttle` fully forward | -100% Throttle

**Tip:** The `forwards` and `back` buttons on `Joystick Hat 3` are mapped to _Forwards_ and _Backwards_. These can be used to temporarily override the throttle setting _100%_ or _0%_.

### Mouse

By default mouse head look is disabled. On screens where the mouse can be used (e.g. station interface and galaxy may) it controls the cursor.

## Button Layout

Please refer to the cheat sheet to identify the various button and hat names.

### Shift Button

`Button 4` on the [Fighterstick][] is used as a `shift` button. Pressing it at the same time as another button will yield the _Shift Action_.

### Fighterstick

#### Buttons

Button  | Action                   | Shift Action
------- | ------------------------ | ------------
`Btn 1` | Primary Fire             | Secondary Fire
`Btn 2` | Toggle Hard Points       | Reset Head Look
`Btn 3` | Primary + Secondary Fire | Fire Chaff
`Btn 4` | `shift`                  | `shift`

**Note:** The `shift` action for `Button 2` is now _Reset Head Look_ not _Fire Chaff_. _Fire Chaff_ is now `shift`+`Btn 3`. `Btn 3` has been given the new function _Primary + Secondary Fire_ which will fire all primary and secondary weapons.

### `POV Hat` - Head Look

The 8-way POV (Point Of View) hat is used to control head look with the 8 directions corresponding to the relevant direction to look in.

**Note:** Head look is now always on (and mouse head look is disabled). Resetting head look is done using `shift`+`btn 2` on the [Fighterstick][].

#### `Hat 1` - Power Management

Direction | Action                     | Shift Action
--------- | -------------------------- | ------------
`Left`    | Divert Power to Systems    | `Macro 1`
`Up`      | Divert Power to Engines    | `Macro 2`
`Right`   | Divert Power to Weapons    | `Macro 3`
`Down`    | Balance Power Distribution | Toggle Silent Running

The three macros configure the ship in the following fashion:

Macro     | Systems | Engines | Weapons
--------- | ------- | ------- | -------
`Macro 1` | 4 Pips  | 2 Pips  | 0 Pips 
`Macro 2` | 2 Pips  | 4 Pips  | 0 Pips
`Macro 3` | 0 Pips  | 2 Pips  | 4 Pips

The macros work by balancing power distribution, then diverting the power as need be. This is literally done by sending the correct key presses in quick succession and so takes a fraction of a second to take effect. You will also notice the visual and audio feedback from the power management panel as the macro runs.

#### `Hat 2` - Targeting

Direction | Action                       | Shift Action
--------- | ---------------------------- | ------------
`Up`      | Select Target Ahead          | Select Next Subsystem
`Down`    | Select Highest Threat        | Select Previous Subsystem
`Left`    | Select Previous Hostile Ship | Select Previous Ship
`Right`   | Select Next Hostile Ship     | Select Next Ship

#### `Hat 3` - Fine ship control

Direction   | Action           | Shift Action
----------- | ---------------- | ------------
`Forwards`  | Thrust Forwards  | Thrust Forwards
`Backwards` | Thrust Backwards | Thrust Backwards
`Left`      | Yaw Left         | Yaw Left
`Right`     | Yaw Right        | Yaw Right

**Note:** `Thrust Forwards` and `Thrust Backwards` temporarily override the `Throttle` setting.

**Tip:** The `Thrust Forwards` and `Thrust Backwards` buttons are primarily used when docking. Once the ship is roughly in the right position over the docking pad throttle back completely. A combination of `Thumb Stick`, `Stick`, and `Hat 3` inputs can be used to provide fine control over positioning or orientation relative to the pad.

**Tip:** `Thrust Backwards` with _Flight Assist Off_ can result in harder braking than simply zeroing the throttle.

### Pro Throttle

#### Buttons

Button  | Action                | Shift Action
------- | --------------------- | ------------
`Btn 4` | UI Select             | UI Back
`Btn 3` | Galaxy Map            | `ESC`
`Btn 2` | Disable Flight Assist | Disable Flight Assist
`Btn 1` | Jettison All Cargo    | Jettison All Cargo

**Note:** The `UI Back` mapping doesn't appear to work in the _Galaxy Map_, however, pressing `Btn 3` again will exit the map.

**Note:** _Galaxy Map_ has been moved from `shift`+`Btn 3` to just `Btn 3`. The _Comms Panel_ mapping is now on `shift`+`Hat 2`. The `ESC` key is now mapped to `shift`+`Btn 3` to allow easier use of the _Comms Panel_.

**Note:** Button 2 will disable flight assist as long as it's held.

**Note:** Button 1 is activated by pressing the thumb stick. I'm aware this is hard to press. It's the reason this has been mapped here.

#### `POV Hat` - Menu Navigation and Wingmen

Direction | Action                | Shift Action
--------- | --------------------- | ------------
`Up`      | UI Panel Up           | Select Wingman 2
`Down`    | UI Panel Down         | Wingman Nav-Lock
`Left`    | UI Panel Previous Tab | Select Wingman 1
`Right`   | UI Panel Next Tab     | Select Wingman 3


**Note:** Only 4 of the possible 8 directions on the throttle POV hat have been mapped. The 4 unmapped directions are simply ignored.

**Note:** This hat now has `shift` actions for wingman control.

**Tip:** The POV hat is designed to be used in conjunction with `Hat 2`, `Hat 3` and `Btn 4` on the throttle.

#### `Hat 1` - Engine Control and Misc Controls

Direction | Action                       | Shift Action
--------- | ---------------------------- | ------------
`Down`    | Boost                        | Toggle Supercruise
`Up`      | Reverse Throttle             | Engage FSD to Hyperspace
`Left`    | Cycle Previous Fire Group    | Decrease Sensor Range
`Right`   | Cycle Next Fire Group        | Increase Sensor Range

**Note:** `shift`+`Down` and `shift`+`Up` are now separate actions for _Supercruise_ and _Hyperspace_ respectively.

#### Hat 2 - UI Panel Select and Misc Controls

Direction | Action        | Shift Action
--------- | --------------| ------------
`Left`    | Target Panel  | Toggle Dev Camera
`Up`      | UI Focus Mode | Comms Panel
`Right`   | Systems Panel | Select Wingman's Target
`Down`    | Radar Panel   | Next System in Route

**Note:** This hat has now acquired `shift` functions 

**Tip:** This hat is mainly used to select a panel to interact with before using the POV hat to then navigate through that panel. Pressing `Up` has the effect of dismissing a panel if one is shown, or giving a slightly wider field of view if no panel is selected. This can be useful for seeing some HUD elements if they're cut off by the edge of the screen.

**Tip:** Selecting a direction a second time will also dismiss the currently displayed panel.

**Tip:** The _Comms Panel_ is now accessed via `shift`+`Up` on this hat. By default the text entry box is not selected. Select it using `Btn 4`. Deselect it by using `shift`+`Btn 3`.

#### Hat 3 - Select and Misc Controls

Direction | Action              | Shift Action
--------- | ------------------- | ------------
`Left`    | UI Left             | Deploy Heat Sink
`Right`   | UI Right            | Use Shield Cell
`Up`      | Toggle Ship Lights  | Toggle Rotational Correction
`Down`    | Toggle Landing Gear | Toggle Cargo Scoop

**Tip:** With the way the UI works, UI Left and UI Right are more like increment and decrement than move left and right, hence mixing and matching Up/Down and Left/Right between Hat 2 and Hat 3

### Mouse

The left mouse button acts like UI Select when the mouse cursor is over a button.

## Keys

Pressing `SPACE` brings up Quick Comms, i.e. a chat entry to the current target. This isn't mapped to a joystick button currently as you'll need to use the keyboard anyway to enter text.

## Navigating The UI

### In Flight

UI Navigation is a little counter intuitive if you simply go by button assignments. In flight you generally use `Hat 2` on the `Throttle` and either `Left` or `Right` to select the relevant UI Panel. The `POV Hat` on the `Throttle` is then used to navigate between tabs and up and down within tabs. `Btn 4` on the `Throttle` is used to select elements. `Left` and `Right` on `Throttle Hat 3` can then be used to alter values that can be altered (for example system priority) and to move between the _Location_ list and map buttons on the _Navigation_ tab. `Forward` and `Back` also moved you between _Fire Groups_ in the _Fire Groups_ tab.

**Tip:** It is also possible to bring up the relevant UI panels with Head Look by looking in the right direction.

### Comms Menu

Use `Left` and `Right` on the `Throttle POV Hat` to navigate the _Comms Menu_. Use Throttle Button 4 to select an action. If the _Text Input_ is selected then use `shift`+`Btn 3` to deselect it. `Up` and `Down` can be used to scroll.

### In Station

The In Flight UI Navigation remains the same in station provided you haven't connected to the Station interface. Once in the station interface use up and down on the `Throttle POV Hat` to move up and down menus, and `Btn 1` on the `Throttle` to select items. `Left` and `Right` on `Throttle Hat 3` can be used for selecting cargo amounts. `shift`+`Throttle Btn 4` can be used to exit the current menu.

You may find it easier to simply use the mouse in station.

### Galaxy Map

A number of overrides are provided for navigating the Galaxy Map. These are:

Control                  | Action
------------------------ | ------
`Joystick Stick Forward` | Pitch Camera Down
`Joystick Stick Back`    | Pitch Camera Up
`Joystick Left`          | Yaw Camera Left
`Joystick Right`         | Yaw Camera Right
`Thumb Stick Up`         | Translate Camera Left
`Thumb Stick Down`       | Translate Camera Right
`Thumb Stick Left`       | Translate Camera Backwards
`Thumb Stick Right`      | Translate Camera Forwards
`Throttle Hat 1 Up`      | Zoom Out
`Throttle Hat 1 Down`    | Zoom In
`Throttle Hat 3 Up`      | Translate Camera Up
`Throttle Hat 3 Down`    | Translate Camera Down

It's generally easier to just use the mouse in the Galaxy Map.

## Landing Overrides

This set up doesn't make use of _Landing Overrides_.

## Joystick Modes

This set up doesn't make use of Joystick modes. The colour of the lit LED on both the stick and the throttle is irrelevant.

## Adding Rudder Pedals

I no longer own the CH Products [Pro Pedals][], however, I have had experience using them. You can add them to this map by clicking the `Add Device` button and selecting the pedals from the list. Order is important in Joystick maps so ensure they are the **3rd** tab, otherwise the CMS script will need to be updated with the new position for the Throttle.

The Axis `Slider 0` and `Slider 1` should be available to bind the yaw axis to, you can then map this in game. The toe pedals can be converted to buttons by copying and adapting the CMS script used for the Throttle Wheel, or you could completely un-map the Throttle wheel and have all three pedal Axis mapped. 

## Possible Future Enhancement

Short of radical control changes or the introduction of several new controls it's unlikely the map will change much. Things that may change are:

* The power setting macros may get a tweak so they provide slightly different settings.
* If we end up with an Iron Man mode and an eject button this may get mapped to `Throtle Btn 1` since cargo can be ejected via the menus.

## TODO

* Add images to this README to make it easier for those not familiar with the [CH Products][] control software.

## About The Author

This was all put together by [Cmdr Davis][]. There's also a [blog][] and [YouTube][] videos relating to [Elite: Dangerous][]. If you see me in game, say "Hi".

## Misc

I found the template I use for printing my joystick cheat sheets years ago on the internet but I've completely forgotten where from. If you can steer my in the correct direction so I can credit the original author I'd greatly appreciate it. 

## Caveat Emptor

With the exception of the PDF all the files contained in this project are text files so, in theory, nothing bad can happen to your system. That said, you're messing about with game config files so if you break anything, you get to keep both halves. If in doubt always back up.

## Changelog

### Version 1.2.0

Improvements for the 1.2 release:
  
  * Headlook is now always on
  * Mouse headlook is disabled
  * Headlook reset has been relocated to `shift`+`btn 2` on the `Stick` (was
    previously `btn 3`)
  * `btn 3` on the `Stick` is now _Fire Primary and Secondary Weapons_
  * `shift`+`btn 3` on the `Stick` is now _Fire Chaff_ (was previously 
    `shift`+`btn 2`)
  * _Galaxy Map_ has been moved to `btn 3` on the `Throttle` (was previously 
    `shift`+`btn 3`)
  * `shift`+`btn 3` on the `Throttle` is now bound to `ESC`
  * The `POV Hat` on the `Throttle` has had _Wingman_ functions mapped to its
    `shift` function
  * `shift`+`Throttle Hat 2 Up` is now _Comms Pannel_ (was previously `btn 3`)
  * `shift`+`Throttle 2 Hat` has had functions mapped to it
  * Tidied up README
  * Change of version numbering to match the version of ED it's intended for

### Version 0.0.5 (Previously version 5)

Improvements for the Gamma release:
  
  * Split Frameshift controls so Hyperdrive and Sepercruise are now seperate 
    buttons
  * Replaced binding to the `ESC` key to the provided `UI Back` control
  * Bound _Galaxy Map_ to a button
  * Bound _Use Shield Cell_ and _Fire Chaff_ to buttons. _Fire Chaff_ replaces 
    _Fire Heat Sync_ on the `Stick` and now lives with  _Use Shield Cell_ on the `Throttle`
  * Minor tweaks to axis direction in the _Galaxy Map_
  * Minor tweaks to the way headlook works with the mouse and bindings
  * Added changelog :)

[previous]: https://github.com/domdavis/ch-products-elite-map/releases/
[CH Products]: http://www.chproducts.com/
[Fighterstick]: http://www.chproducts.com/Fighterstick-v13-d-722.html
[Pro Throttle]: http://www.chproducts.com/Pro-Throttle-v13-d-719.html
[Elite: Dangerous]: http://www.elitedangerous.com/
[zip file]: https://github.com/domdavis/ch-products-elite-map/archive/master.zip
[Control Manager]: http://www.ch-hangar.com/forum/index.php/files/file/49-control-manager/
[Pro Pedals]: http://www.chproducts.com/Pro-Pedals-v13-d-716.html
[Cmdr Davis]: https://twitter.com/cmdr_davis 
[blog]: http://elite.domdavis.com
[YouTube]: https://www.youtube.com/user/idomdavis
