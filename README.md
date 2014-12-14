# CH Products Joystick Map for Elite: Dangerous

Joystick maps and game configuration files for the [CH Products][] [Fighterstick][] and [Pro Throttle][] HOTAS in [Elite: Dangerous][].

## About

These maps are my own personal configuration that I've put together while playing the Elite: Dangerous Alpha and Beta. The maps have evolved over time and are presented here as it's a much easier way of distributing changes. As the game evolves and my play style evolves you may see additional changes. Feel
free to download, use and tweak for your own setup.

## Requirements

* [CH Products][] [Fighterstick][]
* [CH Products][] [Pro Throttle][]
* [CH Products][] [Control Manager][] software
* [Elite: Dangerous][]
* Optional: PDF viewer

## Installation

* Download and extract the [zip file][] containing the game files.

### Joystick Maps

Navigate to `My Documents` and create a folder called `CH Control Manager` if it doesn't already exist.

Within the extracted zip file under the `maps` folder you'll find two files
called `elite.cms` and `elite.map`. These need to be copied to the `CH Control Manager` folder.

Plugin your [Fighterstick][] and [Pro Throttle][], then launch the [CH Control Manager][Control Manager] and load the `elite.map`. The load dialog should default to the folder you copies your maps to, if it doesn't just navigate to that folder. Once loaded click the `Download` button to enable the map.

### Game Configuration

Within the extracted zip file under the `config` folder you'll find two files called `Custom.binds` and `StartPreset.start`. Copy `Custom.binds` to
`C:\Users\USER\AppData\Local\Frontier Developments\Elite Dangerous\Options\Bindings\Custom.binds`. Change `USER` to be your username. `AppData` is a hidden folder so you’ll need to enable _Show Hidden Files_ to see it.

You can optionally copy `StartPreset.start` to the same folder. All this does is tell the game to use the custom bindings by default. If you don't copy the file you'll need select the custom layout from within the game under the input settings.

## Cheat Sheet

Within the root of the extracted zip file you'll find a file called `layout.pdf`. This file contains the button layout for the joystick map which can be used as a cheat sheet.

## Axis Layout

### Fighterstick

Axis             | Action
---------------- | ------
Pitch down       | Stick forward
Pitch up         | Stick back
Roll left        | Stick left
Roll right       | Stick right
Enable Throttle  | Throttle wheel forward<sup>1</sup>
Disable Throttle | Throttle wheel back<sup>1</sup>

> <sup>1</sup> The throttle wheel on the stick is used to enable and disable analogue throttle inputs from the [Pro Throttle][]. This allows you to bring the ship to a full stop even if your throttle is suffering from drift and not returning completely to zero when fully back. With the wheel moved back input from the [Pro Throttle][] is ignored and a throttle setting of zero (full stop) is used. With the wheen moved forward the [Pro Throttle][] is enabled. You should ensure the throttle wheel is fully forward if the [Pro Throttle][] is not responding.  

### Pro Throttle

Axis          | Action
------------- | ------
0% Throttle   | Throttle fully back
100% Throttle | Throttle fully forward
Thrust Up     | Thumb stick up
Thrust Down   | Thumb stick down
Thrust Left   | Thumb stick left
Thrust Right  | Thumb stick right 

**Note:** Analogue inputs for reverse thrust (0% to -100%) are achieved by holding the back button on the front 4-way hat on the throttle. With this button held the mappings for the throttle axis become

Axis           | Action
-------------- | ------
0% Throttle    | Throttle fully back
-100% Throttle | Throttle fully forward

### Mouse

By default the mouse is used to control head look. On screens where the mouse can be used (e.g. station interface and galaxy may) the mouse is then used to control the cursor.

## Button Layout

Please refer to the cheat sheet to identify the various button and hat names.

### Shift Button

`Button 4` on the [Fighterstick][] is used as a `shift` button. Pressing it at the same time as another button will yield the _shift action_.

### Fighterstick

#### Buttons

Button | Action             | Shift Action
------ | ------------------ | ------------
Btn 1  | Primary Fire       | Secondary Fire
Btn 2  | Toggle Hard Points | Fire Chaff
Btn 3  | Reset Head Look    | Toggle Head Look
Btn 4  | Shift              | Shift

_Note:_ The `shift` action for `Button 2` is now _Fire Chaff_ not _Launch Heat Sink_. _Launch Heat Sink_ is now `Hat 3` of the [Pro Throttle][].

### POV Hat - Head Look

The 8-way POV (Point Of View) hat is used to control head look with the 8 directions corresponding to the relevant direction to look in.

#### Hat 1 - Power Management

Direction | Action                     | Shift Action
--------- | -------------------------- | ------------
Left      | Divert Power to Systems    | `Macro 1`
Up        | Divert Power to Engines    | `Macro 2`
Right     | Divert Power to Weapons    | `Macro 3`
Down      | Balance Power Distribution | Toggle Silent Running

The three macros configure the ship in the following fashion:

Macro   | Systems | Engines | Weapons
------- | ------- | ------- | -------
Macro 1 | 4 Pips  | 2 Pips  | 0 Pips 
Macro 2 | 2 Pips  | 4 Pips  | 0 Pips
Macro 3 | 0 Pips  | 2 Pips  | 4 Pips

The macros work by balancing power distribution, then diverting the power as need be. This is literally done by sending the correct key presses in quick succession and so takes a fraction of a second to take effect. You will also notice the visual and audio feedback from the power management panel as the macro runs.

#### Hat 2 - Targeting

Direction | Action                       | Shift Action
--------- | ---------------------------- | ------------
Up        | Select Target Ahead          | Select Next Subsystem
Down      | Select Highest Threat        | Select Previous Subsystem
Left      | Select Previous Hostile Ship | Select Previous Ship
Right     | Select Next Hostile Ship     | Select Next Ship

#### Hat 3 - Fine ship control

Direction | Action           | Shift Action
--------- | ---------------- | ------------
Forwards  | Thrust Forwards  | Thrust Forwards
Backwards | Thrust Backwards | Thrust Backwards
Left      | Yaw Left         | Yaw Left
Right     | Yaw Right        | Yaw Right

The `Thrust Forwards` and `Thrust Backwards` buttons are primarily used when docking. Once the ship is roughly in the right position over the docking pad throttle back completely. A combination of Thumb stick, stick, and Hat 3 inputs can be used to provide fine control over positioning or orientation relative to the pad.

### Pro Throttle

#### Buttons

Button | Action                | Shift Action
------ | --------------------- | ------------
Btn 4  | UI Select             | UI Back
Btn 3  | Comms Panel           | Galaxy Map
Btn 2  | Disable Flight Assist | Disable Flight Assist
Btn 1  | Jettison All Cargo    | Jettison All Cargo

With the addition of `UI Back` the shifted action for button 4 has been mapped to this. Currently there is no longer any way to bring up the 'Pause Menu' in game so you'll need to use `ESC` on the keyboard. The `UI Back` mapping doesn't appear to work in the _Galaxy Map_, however, pressing `shift` `Button 3` again will exit the map.

Button 2 will disable flight assist as long as it's held.

Button 1 is activated by pressing the thumb stick.

#### POV Hat - Menu Navigation

Direction | Action                | Shift Action
--------- | --------------------- | ------------
Up        | UI Panel Up           | Select Next Subsystem
Down      | UI Panel Down         | Select Previous Subsystem
Left      | UI Panel Previous Tab | Select Previous Ship
Right     | UI Panel Next Tab     | Select Next Ship


Only 4 of the possible 8 directions on the throttle POV hat have been mapped. The 4 unmapped directions are simply ignored.

The POV hat is designed to be used in conjunction with Hat 2, Hat 3 and Button 4 on the throttle.

#### Hat 1 - Engine Control and Misc Controls

Direction | Action                       | Shift Action
--------- | ---------------------------- | ------------
Down      | Boost                        | Toggle Frame Shift Drive
Up        | Reverse Throttle             | Toggle Frame Shift Drive
Left      | Cycle Previous Fire Group    | Decrease Sensor Range
Right     | Cycle Next Fire Group        | Increase Sensor Range

There is no difference between Shift + Up or Shift + Down, currently they're provided to allow the feeling of "engaging" and "disengaging" the drive. Shift + Up may get used for another function in future revisions.

#### Hat 2 - UI Panel Select

Direction | Action        | Shift Action
--------- | --------------| ------------
Left      | Target Panel  | Target Panel
Up        | UI Focus Mode | UI Focus Mode
Right     | Systems Panel | Systems Panel
Down      | Radar Panel   | Radar Panel

This hat is used to select a panel to interact with before using the POV hat to then navigate through that panel. Pressing Up has the effect of dismissing a panel if one is shown, or giving a slightly wider field of view if no panel is selected. This can be useful for seeing some HUD elements if they're cut off by the edge of the screen.

Selecting a direction a second time will also dismiss the currently displayed panel.

#### Hat 3 - Select and Misc Controls

Direction | Action              | Shift Action
--------- | ------------------- | ------------
Left      | UI Left             | Deploy Heat Sink
Right     | UI Right            | Use Shield Cell
Up        | Toggle Ship Lights  | Toggle Rotational Correction
Down      | Toggle Landing Gear | Toggle Cargo Scoop

With the way the UI works, UI Left and UI Right are more like increment and decrement than move left and right, hence mixing and matching Up/Down and Left/Right between Hat 2 and Hat 3

### Mouse

The left mouse button acts like UI Select when the mouse cursor is over a button.

## Keys

Pressing `SPACE` brings up Quick Comms, i.e. a chat entry to the current target. This isn't mapped to a joystick button currently as you'll need to use the keyboard anyway to enter text.

## Navigating The UI

### In Flight

UI Navigation is a little counter intuitive if you simply go by button assignments. In flight you generally use Hat 2 on the Throttle and either left or right to select the relevant UI Panel. The POV Hat on the Throttle is then used to navigate between tabs and up and down within tabs. Button 4 on the Throttle is used to select elements. Left and Right on Throttle Hat 3 can then be used to alter values that can be altered (for example system priority). Forward and Back also moved you between Fire Groups in the Fire Groups tab.

It is also possible to bring up the relevant UI panels with Head Look by looking in the right direction.

### Comms Menu

Use Up and Down on the Throttle POV Hat to navigate the Comms Menu. Use Throttle Button 4 to select an action.

### In Station

The In Flight UI Navigation remains the same in station provided you haven't connected to the Station interface. Once in the station interface use up and down on the Throttle POV Hat to move up and down menus, and button 1 on the throttle to select items. Left and Right on Throttle Hat 3 can be used for selecting cargo amounts. Shift and Throttle Button 4 can be used to exit the current menu.

You may find it easier to simply use the mouse in station.

### Galaxy Map

A number of overrides are provided for navigating the Galaxy Map. These are:

Control                | Action
---------------------- | ------
Joystick Stick Forward | Pitch Camera Down
Joystick Stick Back    | Pitch Camera Up
Joystick Left          | Yaw Camera Left
Joystick Right         | Yaw Camera Right
Thumb Stick Up         | Translate Camera Left
Thumb Stick Down       | Translate Camera Right
Thumb Stick Left       | Translate Camera Backwards
Thumb Stick Right      | Translate Camera Forwards
Throttle Hat 1 Up      | Zoom Out
Throttle Hat 1 Down    | Zoom In
Throttle Hat 3 Up      | Translate Camera Up
Throttle Hat 3 Down    | Translate Camera Down

It's generally easier to just use the mouse in the Galaxy Map.

## Landing Overrides

This set up doesn't make use of _Landing Overrides_.

## Joystick Modes

This set up doesn't make use of Joystick modes. The colour of the lit LED on both the stick and the throttle is irrelevant.

## Adding Rudder Pedals

I no longer own the CH Products [Pro Pedals][], however, I have had experience using them. You can add them to this map by clicking the `Add Device` button and selecting the pedals from the list. Order is important in Joystick maps so ensure they are the **3rd** tab, otherwise the CMS script will need to be updated with the new position for the Throttle.

The Axis `Slider 0` and `Slider 1` should be available to bind the yaw axis to, you can then map this in game. The toe pedals can be converted to buttons by copying and adapting the CMS script used for the Throttle Wheel, or you could completely un-map the Throttle wheel and have all three pedal Axis mapped. 

## Possible Future Enhancement

This is version 5 of my Elite Dangerous map and the fourth I've published. Short of radical control changes or the introduction of several new controls before the final release it's unlikely the map will change much. That said a few ideas I have kicking about are:

* Map Throttle Hat 1 Up to a landing macro that will deploy landing gear and set 1 pip to engines (with probably 4 pips to systems and the last pip popped into weapons). At the moment I'm happy landing with 2 pips in engines but the Type 9 and the Anaconda may want slower approaches.
* Map Throttle Hat 1 Down so that disables flight assist for as long as it's pressed. Since I generally boost with flight assist off this saves having to press two buttons.
* Map Button 3 so that the Shift action is to open Quick Comms

## TODO

* Add images to this README to make it easier for those not familiar with the [CH Products][] control software.

## About The Author

This was all put together by [Cmdr Davis][]. There's also a [blog][] and [YouTube][] videos relating to [Elite: Dangerous][]. If you see me in game, say "Hi".

## Misc

I found the template I use for printing my joystick cheat sheets years ago on the internet but I've completely forgotten where from. If you can steer my in the correct direction so I can credit the original author I'd greatly appreciate it. 

## Caveat Emptor

With the exception of the PDF all the files contained in this project are text files so, in theory, nothing bad can happen to your system. That said, you're messing about with game config files so if you break anything, you get to keep both halves. If in doubt always back up.

## Changelog

### Version 5

Improvements for the Gamma release:
  
  * Split Frameshift controls so Hyperdrive and Sepercruise are now seperate buttons
  * Replaced binding to the `ESC` key to the provided `UI Back` control
  * Bound _Galaxy Map_ to a button
  * Bound _Use Shield Cell_ and _Fire Chaff_ to buttons. _Fire Chaff_ replaces _Fire Heat Sync_ on the [Fighterstick][] and now lives with _Use Shield Cell_ on the [Pro Throttle][]
  * Minor tweaks to axis direction in the _Galaxy Map_
  * Minor tweaks to the way headlook works with the mouse and bindings
  * Added changelog :)


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
