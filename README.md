# CH Products Joystick Map for Elite: Dangerous

Joystick maps and game configuration files for the [CH Products][] [Fighterstick][] and [Pro Throttle][] HOTAS in [Elite: Dangerous][].

## About

These maps are my own personal configuration that I've put together while playing Elite: Dangerous. The maps have evolved over time and are presented here as it's a much easier way of distributing changes. As the game evolves and my play style evolves you may see additional changes. Feel free to download, use and tweak for your own setup.

### Version

This version of the map is designed for use with Elite: Dangerous 1.2.03 and above.

This map introduces a new modifier button (the `alt` button), tightens up much of the grouping that was set in previous versions, and moves some button assignments around to facilitate this. 

Notes are included below to indicate changes from previous maps. It is also recommended you study the [Layout][pdf] before flying with this map. 

> **Note:** The map is almost entirely virtual. Most definitions are done via CMS rather than direct mappings on the devices.

### Previous versions

Previous versions of the joystick maps, including the relevant README.md and layout guides, can be found [here][previous]. Major version number changes indicate complete overhauls of the map.

## Requirements

* [CH Products][] [Fighterstick][]
* [CH Products][] [Pro Throttle][]
* [CH Products][] [Control Manager][] software
* [Elite: Dangerous][] 1.2.03 or above
* Optional: PDF viewer

## Installation

Download and extract the [zip file][] containing the game files.

### Joystick Maps

Navigate to `My Documents` and create a folder called `CH Control Manager` if it doesn't already exist, and under it a folder called `Maps`.

Within the extracted zip file under the `maps` folder you'll find two files
called `elite.cms` and `elite.map`. These need to be copied to the `CH Control Manager/Maps` folder.

![The load dialog](images/load.png)

Plugin your [Fighterstick][] and [Pro Throttle][], then launch the [CH Control Manager][Control Manager]. Load the `elite.map`. The load dialog should default to the folder you copied your maps to. If it doesn't just navigate to that folder. 

![The Download Button](images/download.png)

Once loaded click the `Download` button to enable the map.

### Game Configuration

Within the extracted zip file under the `config` folder you'll find two files called `Custom.binds` and `StartPreset.start`. Copy `Custom.binds` to
`C:\Users\USER\AppData\Local\Frontier Developments\Elite Dangerous\Options\Bindings\Custom.binds`. Change `USER` to be your username. `AppData` is a hidden folder so you’ll need to enable _Show Hidden Files_ to see it.

You can optionally copy `StartPreset.start` to the same folder. All this does is tell the game to use the custom bindings by default. If you don't copy the file you'll need select the custom layout from within the game under the input settings.

## Cheat Sheet

Within the root of the extracted zip file you'll find a file called `layout.pdf`. This file contains the button layout for the joystick map which can be used as a cheat sheet.

## Conventions

This document uses a few basic conventions. Buttons and Axis are denoted using `fixed width` type. In game actions are given in _italics_ . Button and hat numbers can be found on the Cheat Sheet.

The [Fighterstick][] is referred to as `Stick` and the [Pro Throttle][] is referred to as `Throttle`.

Axis are referred to using `Device axis` where `axis` is either `x`, `y` or `z`. `Stick x` and `Stick y` are left/right and forward/back respectively. `Stick z` is the throttle wheel. `Throttle x` and `Throttle y` are mini-stick left/right and mini-stick up/down respectively. `Throttle z` is the throttle axis. 

Individual buttons are referred to using the format `Btn n` where `n` is the button number from the cheat sheet. This can be prefixed with `Throttle` or `Stick`.

Hats are referred to using the format `Hat n` where `n` is the hat number from the cheat sheet. This can be prefixed with `Throttle` or `Stick`.

Individual hat buttons are referred to using the direction you need to move the hat to activate the button. For most hats this is `Up`, `Down`, `Left` and `Right`. The exception here is `Stick Hat 3` which uses `Forwards` and `Backwards` instead of `Up` and `Down`.

POV Hat buttons are referred to in a similar way to hats, except they use `POV` instead of `Hat n`. For example: `Stick POV Up`.

Modifier buttons are referred to as `shift` (`Stick Btn 4`) and `alt` (`Throttle Btn 3`). Where a modifier is used it is written as `modifier` + `button` where `modifier` is either `shift` or `alt`, and `button` is the button or hat switch to press at the same time. Modifiers can stack, so `shift` + `alt` + `button` is valid and means you need to press 3 buttons to achieve the effect.

## Axis Layout

### Fighterstick

Axis      | Action
--------- | ------
`Stick x` | _Roll left/right_
`Stick y` | _Pitch up/down_
`Stick z` | _Scanner Range_<sup>[1]</sup>

Notes:
> <sup>[1]</sup> Previously `Stick z` disabled and enabled `Throttle z`. `Throttle z` is now toggled on and off by `alt`+`Throttle Hat 1 Left`.

### Pro Throttle

Axis         | Action
------------ | ------
`Throttle x` | _Thrust left/right_
`Throttle y` | _Thrust up/down_
`Throttle z` | _Throttle_ (0%-100%)<sup>[1], [2]</sup>

Notes:
> <sup>[1]</sup> Reverse thrust (0% to -100%) using the `Throttle` can be achieved by holding `Throttle Hat 1 Up`.

> <sup>[2]</sup> `Stick hat 3 Forward` and `Stick Hat 3 Back` are mapped to _Thrust Forwards_ and _Thrust Backwards_ respectively. These override the `Throttle` setting while pressed and allow for digital control when docking, 'blipping' the throttle, and emergency reverse without touching the throttle.

### Mouse

By default mouse head-look is disabled. On screens where the mouse can be used (e.g. station interface and galaxy may) it controls the cursor.

## Button Layout

### Modifier Buttons

Button           | Modifier
---------------- | --------
`Stick Btn 4`    | `shift`
`Throttle Btn 3` | `alt`

### Fighterstick

#### Buttons

Trigger (`Btn 1`)         | Action                     
------------------------- | ------
`Btn 1`                   | _Primary Fire_
`shift` + `Btn 1`         | _Secondary Fire_
`alt` + `Btn 1`           | _Primary + Secondary Fire_<sup>[1]</sup>
`shift` + `alt` + `Btn 1` | _Primary + Secondary Fire_<sup>[1]</sup>

Button 2 (`Btn 2`)        | Action                     
------------------------- | ------
`Btn 2`                   | _Toggle Hard Points_
`shift` + `Btn 2`         | _Toggle Hard Points_<sup>[2]</sup>
`alt` + `Btn 2`           | _Toggle Hard Points_
`shift` + `alt` + `Btn 2` | _Toggle Silent Running_<sup>[3]</sup>

Countermeasures (`Btn 3`) | Action                     
------------------------- | ------
`Btn 3`                   | _Fire Chaff_<sup>[4]</sup>
`shift` + `Btn 3`         | _Use Shield Cell_<sup>[5]</sup>
`alt` + `Btn 3`           | _Deploy Heat Sink_<sup>[6]</sup>
`shift` + `alt` + `Btn 3` | _Deploy Heat Sink_<sup>[6]</sup>

Notes:
> <sup>[1]</sup> Moved from `Stick Btn 3`<br/>
> <sup>[2]</sup> _Reset Head-Look_ is now `shift`+`Stick POV Up`<br/>
> <sup>[3]</sup> Moved from `shift`+`Stick Hat 1 Down`<br/>
> <sup>[4]</sup> Moved from `shift`+`Stick Btn 3`<br/>
> <sup>[5]</sup> Moved from `shift`+`Throttle Hat 3 Right`<br/>
> <sup>[6]</sup> Moved from `shift`+`Throttle Hat 4 Left`<br/>

### Head-Look (`POV Hat`)

`Stick POV` is used to control head-look with the 8 directions corresponding to the relevant direction to look in. Head-Look is now always on (and mouse head-look is disabled). `Stick POV` also has some modified button assignments. These are:

Reset (`POV Up`)                 | Action
-------------------------------- | ------
`shift` + `POV Up`               | _Reset Head-Look_<sup>[2]</sup>
`alt` + `POV Up`                 | _Toggle Head-Look_
`shift` + `alt` + `POV Up`       | _Reset Oculus Orientation_

Dev Camera (`POV Down`)          | Action
-------------------------------- | ------
`alt` + `POV Down`               | _Toggle Dev Camera_<sup>[3]</sup>
`shift` + `alt` + `POV Down`     | _Toggle Recording_<sup>[4]</sup>

Screen Shot (`POV Left`)         | Action
-------------------------------- | ------
`shift` + `POV Left`             | _Screen Shot_
`alt` + `POV Left`               | _Screen Shot_
`shift` + `alt` + `POV Left`     | _Screen Shot_

Hi-Res Screen Shot (`POV Right`) | Action
-------------------------------- | ------
`shift` + `POV Right`            | _High ResolutionScreen Shot_
`alt` + `POV Right`              | _High ResolutionScreen Shot_
`shift` + `alt` + `POV Right`    | _High ResolutionScreen Shot_

Notes:
> <sup>[1]</sup> All other combinations are mapped to the 8 directions corresponding to the relevant direction to look in<br/>
> <sup>[2]</sup> Moved from `shift`+`Stick Btn 2` (and `Stick Btn 3` before that)<br/>
> <sup>[3]</sup> Moved from `Throttle Hat 2 Left`<br/>
> <sup>[4]</sup> I use NVidia ShadowPlay mapped to `ALT` + `F9` to record playing. Feel free to ignore this mapping, or use it for something else bound to the same key combination

#### Power Management (`Hat 1`)

Systems (`Left`)          | Action
------------------------- | ------
`Left`                    | _Divert Power to Systems_ 
`shift` + `Left`          | `Preset: Systems 1`
`alt` + `Left`            | `Preset: Systems 2`<sup>[1]</sup>
`shift` + `alt` + `Left`  | `Preset: Systems 3`<sup>[1]</sup>

Engines (`Up`)            | Action
------------------------- | ------
`Up`                      | _Divert Power to Engines_ 
`shift` + `Up`            | `Preset: Engines 1`
`alt` + `Up`              | `Preset: Engines 2`<sup>[1]</sup>
`shift` + `alt` + `Up`    | `Preset: Engines 3`<sup>[1]</sup>

Weapons (`Right`)         | Action
------------------------- | ------
`Right`                   | _Divert Power to Engines_ 
`shift` + `Right`         | `Preset: Weapons 1`
`alt` + `Right`           | `Preset: Weapons 2`<sup>[1]</sup>
`shift` + `alt` + `Right` | `Preset: Weapons 3`<sup>[1]</sup>

Balance/Misc (`Down`)     | Action
------------------------- | ------
`Down`                    | _Balance Power Distribution_
`shift` + `Down`          | `Preset: Misc 1`<sup>[2]</sup>
`alt` + `Down`            | `Preset: Misc 2`<sup>[1]</sup>
`shift` + `alt` + `Down`  | `Preset: Misc 3`<sup>[1]</sup>

Notes:
> <sup>[1]</sup> New presets added in this version<br/>
> <sup>[2]</sup> _Toggle Silent Running_ has moved to `alt`+`Stick Btn 2`<br/>

The presets configure the ship in the following fashion:

Preset              | Systems  | Engines  | Weapons
------------------- | -------- | -------- | -------
`Preset: Systems 1` | 4 Pips   | 2 Pips   | 0 Pips
`Preset: Systems 2` | 4 Pips   | 1 Pip    | 1 Pip
`Preset: Systems 3` | 3 Pips   | 1.5 Pips | 1.5 Pips
`Preset: Engines 1` | 2 Pips   | 4 Pips   | 0 Pips
`Preset: Engines 2` | 1 Pip    | 4 Pips   | 1 Pip
`Preset: Engines 3` | 1.5 Pips | 3 Pips   | 1.5 Pips
`Preset: Weapons 1` | 0 Pips   | 2 Pips   | 4 Pips
`Preset: Weapons 2` | 1 Pip    | 1 Pip    | 4 Pips
`Preset: Weapons 3` | 1.5 Pips | 1.5 Pips | 3 Pips
`Preset: Misc 1`    | 1 Pip    | 2.5 Pips | 2.5 Pips
`Preset: Misc 2`    | 2.5 Pips | 1 Pip    | 2.5 Pips
`Preset: Misc 3`    | 2.5 Pips | 2.5 Pips | 1 Pip

> **Note:** The presets work by balancing power distribution, then diverting the power as need be. This is literally done by sending the correct key presses in quick succession and so takes a fraction of a second to take effect. You will also notice the visual and audio feedback from the power management panel as the macro runs.

#### Targeting (`Hat 2`)

Direction: `Up`           | Action
------------------------- | ------
`Up`                      | _Select Target Ahead_
`shift` + `Up`            | _Select Next Subsystem_
`alt` + `Up`              | _Select Wingman's Target_<sup>[1]</sup>
`shift` + `alt` + `Up`    | _Select Wingman's Target_<sup>[1]</sup>

Direction: `Down`         | Action
------------------------- | ------
`Down`                    | _Select Highest Threat_
`shift` + `Down`          | _Select Previous Subsystem_
`alt` + `Down`            | _Next System In Route_<sup>[2]</sup>
`shift` + `alt` + `Down`  | _Next System In Route_<sup>[2]</sup>

Direction: `Left`         | Action
------------------------- | ------
`Left`                    | _Select Previous Hostile Ship_
`shift` + `Left`          | _Select Previous Ship_
`alt` + `Left`            | _Select Previous Ship_
`shift` + `alt` + `Left`  | _Select Previous Ship_

Direction: `Right`        | Action
------------------------- | ------
`Right`                   | _Select Next Hostile Ship_
`shift` + `Right`         | _Select Next Ship_
`alt` + `Right`           | _Select Next Ship_
`shift` + `alt` + `Right` | _Select Next Ship_

Notes:
> <sup>[1]</sup> Moved from `shift`+`Throttle Hat 2 Right`<br/>
> <sup>[2]</sup> Moved from `shift`+`Throttle Hat 2 Down`<br/>

#### Fine ship control (`Hat 3`)

Direction   | Action<sup>[1]</sup> 
----------- | --------------------
`Forwards`  | _Thrust Forwards_<sup>[2]</sup>
`Backwards` | _Thrust Backwards_<sup>[2],[3]</sup>
`Left`      | _Yaw Left_
`Right`     | _Yaw Right_

Notes:
> <sup>[1]</sup> These buttons always have the same action, regardless of modifier button.

> <sup>[2]</sup> _Thrust Forwards_ and _Thrust Backwards_ override the `Throttle` setting while pressed and allow for digital control when docking. A combination of `Throttle x`, `Throttle y`, `Stick`, and `Stick Hat 3` inputs can be used to provide fine control over positioning or orientation relative to the pad.

> <sup>[3]</sup> _Thrust Backwards_ with _Flight Assist Off_ can result in harder braking than simply zeroing the throttle.

### Pro Throttle

#### Buttons

UI Actions (`Btn 4`)      | Action
------------------------- | ------
`Btn 4`                   | _UI Select_
`shift` + `Btn 4`         | _UI Back_<sup>[1]</sup>
`alt` + `Btn 4`           | `ESC`<sup>[2]</sup>
`shift` + `alt` + `Btn 4` | _Game Menu_

Other Buttons             | Action
------------------------- | ------
`Btn 1`                   | Not Used<sup>[3]</sup>
`Btn 2`                   | _Disable Flight Assist_<sup>[4]</sup>
`Btn 3`                   | `alt`<sup>[5]</sup>
`shift` + `Btn 3`         | `shift` + `alt`<sup>[6]</sup>

Notes:
> <sup>[1]</sup> Doesn't exit _Galaxy Map_, use `shift` + `Throttle Hat 2 Left`<br/>
> <sup>[2]</sup> Previously `Throttle Btn 3`<br/>
> <sup>[3]</sup> _Jettison All Cargo_ is now `alt` + `shift` + `Throttle Hat 3 Down`<br/>
> <sup>[4]</sup> Will disable flight assist as long as it's held<br/>
> <sup>[5]</sup> _Galaxy Map_ is now `shift` + `Throttle Hat 2 Left`<br/>
> <sup>[6]</sup> `ESC` is now `alt` + `Btn 4`<br/>

#### Menu Navigation (`POV Hat`)

> **Note:** Only 4 of the possible 8 directions on the throttle POV hat have been mapped. The 4 unmapped directions are simply ignored.

> **Tip:** With the way the UI works, UI Left and UI Right are more like _Increment_/_Decrement_ and _Panel Left_/_Right_ than move left and right hence mixing and matching Up/Down and Left/Right between unmodified/modified and having _Next_/_Previous Tab_ unmodified.

Direction | Action                  | Modified Action<sup>[1]</sup>
--------- | ----------------------- | -----------------------------
`Up`      | _UI Panel Up_           | _UI Panel Up_<sup>[2]</sup>
`Down`    | _UI Panel Down_         | _UI Panel Down_<sup>[3]</sup>
`Left`    | _UI Panel Previous Tab_ | _UI Panel Left_<sup>[4], [5]</sup>
`Right`   | _UI Panel Next Tab_     | _UI Panel Right_<sup>[6], [7]</sup>

Notes:
> <sup>[1]</sup> Actions work with `shift`, `alt`, and `shift` + `alt`<br/>
> <sup>[2]</sup> _Select Wingman 2_ is now `Throttle Hat 3 Up`<br/>
> <sup>[3]</sup> _Wingman Nav-Lock_ is now `shift` + `Throttle Hat 3 Up`<br/>
> <sup>[4]</sup> _Select Wingman 1_ is now `Throttle Hat 3 Left`<br/>
> <sup>[5]</sup> Previously `Throttle Hat 3 Left`<br/>
> <sup>[6]</sup> _Select Wingman 3_ is now `Throttle Hat 3 Right`<br/>
> <sup>[7]</sup> Previously `Throttle Hat 3 Right`<br/>

#### Engine Control and Misc Controls (`Hat 1`)

Direction: `Up`           | Action
------------------------- | ------
`Up`                      | _Reverse Throttle_
`shift` + `Up`            | _Toggle Hyperdrive_
`alt` + `Up`              | _Toggle Rotational Correct_<sup>[1]</sup>
`shift` + `alt` + `Up`    | _Toggle Rotational Correct_<sup>[1]</sup>

Direction: `Down`         | Action
------------------------- | ------
`Down`                    | _Boost_
`shift` + `Down`          | _Toggle Supercruise_
`alt` + `Down`            | _Toggle Ships Lights_<sup>[2]</sup>
`shift` + `alt` + `Down`  | _Toggle Ships Lights_

Direction: `Left`         | Action
------------------------- | ------
`Left`                    | _Previous Fire Group_
`shift` + `Left`          | _Previous Fire Group_<sup>[3]</sup>
`alt` + `Left`            | _Disable/Enable`Throttle`_<sup>[4]</sup>
`shift` + `alt` + `Left`  | _Show FPS_

Direction: `Right`        | Action
------------------------- | ------
`Right`                   | _Next Fire Group_
`shift` + `Right`         | _Next Fire Group_<sup>[3]</sup>
`alt` + `Right`           | _Toggle Roll/Yaw_<sup>[5]</sup>
`shift` + `alt` + `Right` | _Show Network Details_

Notes:
> <sup>[1]</sup> Previously `shift` + `Throttle Hat 3 Up`<br/>
> <sup>[2]</sup> Previously `Throttle Hat 3 Up`<br/>
> <sup>[3]</sup> _Scanner Range_ is now `Stick z`<br/>
> <sup>[4]</sup> Previously `Stick z`<br/>
> <sup>[5]</sup> Toggles `Stick x` between _Roll_ and _Yaw_ <br/>

#### UI Panels/Maps (`Hat 2`)

> **Tip:** This hat is mainly used to select a panel to interact with before using the POV hat to then navigate through that panel. Pressing `Up` has the effect of dismissing a panel if one is shown, or giving a slightly wider field of view if no panel is selected. This can be useful for seeing some HUD elements if they're cut off by the edge of the screen.

> **Tip:** Selecting a direction a second time will also dismiss the currently displayed panel.

Direction | Action          | Modified Action<sup>[1]</sup>
--------- | ----------------| -----------------------------
`Up`      | _UI Focus Mode_ | _Comms Panel_<sup>[2]</sup>
`Down`    | _Radar Panel_   | _Mute/Unmute Microphone_
`Left`    | _Target Panel_  | _Galaxy Map_<sup>[3]</sup>
`Right`   | _Systems Panel_ | _System Map_

Notes:
> <sup>[1]</sup> Actions work with `shift`, `alt`, and `shift` + `alt`<br/>
> <sup>[1]</sup> By default the text entry box is not selected. Select it using `Btn 4`. Deselect it by using `shift` + `alt` + `Btn 3`<br/>
> <sup>[3]</sup> Previously `Throttle Btn 3` (and `shift` + `Throttle Btn 3` prior to that)<br/>


#### Wingmen (`Hat 3`)

Direction | Action                           | Modified Action<sup>[1]</sup>
--------- | -------------------------------- | -----------------------------
`Left`    | _Select Wingman 1_<sup>[2]</sup> | _Select Wingman 1_
`Up`      | _Select Wingman 2_<sup>[3]</sup> | _Wingman Nav-Lock_<sup>[5]</sup>
`Right`   | _Select Wingman 3_<sup>[4]</sup> | _Select Wingman 3_

Notes:
> <sup>[1]</sup> Actions work with `shift`, `alt`, and `shift` + `alt`<br/>
> <sup>[2]</sup> Previously `shift` + `Throttle POV Left`<br/>
> <sup>[3]</sup> Previously `shift` + `Throttle POV Up`<br/>
> <sup>[4]</sup> Previously `shift` + `Throttle POV Right`<br/>
> <sup>[5]</sup> PReviously `shift` + `Throttle POV Down`<br/>

#### Landing Gear and Cargo (`Hat 3`)

Button                   | Action
------------------------ | ------
`Down`                   | _Toggle Landing Gear_
`shift` + `Down`         | _Toggle Cargo Scoop_
`alt` + `Down`           | _Toggle Cargo Scoop_
`shift` + `alt` + `Down` | _Jettison All Cargo_<sup>[1]</sup>

Notes:
> <sup>[1]</sup> Previously `Throttle Btn 1`<br/>

### Mouse

The left mouse button acts like UI Select when the mouse cursor is over a button.

## Keys

Pressing `SPACE` brings up Quick Comms, i.e. a chat entry to the current target. This isn't mapped to a joystick button currently as you'll need to use the keyboard anyway to enter text.

## Navigating The UI

### In Flight

UI Navigation is a little counter intuitive if you simply go by button assignments. In flight you generally use `Throttle Hat 2` and either `Left` or `Right` to select the relevant UI Panel. `Throttle POV` is then used to navigate between tabs and up and down within tabs with `Throttle Btn 4` used to select elements. `shift` + `Throttle POV Left` and `Right` can then be used to alter values that can be altered (for example system priority) and to move between sub-panels (e.g. the _Location_ list and map buttons on the _Navigation_ tab, and _Fire Groups_ in the _Fire Groups_ tab).

> **Tip:** It is also possible to bring up the relevant UI panels with Head Look by looking in the right direction.

### Comms Menu

Use `Left` and `Right` on the `Throttle POV Hat` to navigate the _Comms Menu_. Use `Throttle Btn 4` to select an action. If the _Text Input_ box is selected then use `shift` + `alt` + `Throttle Btn 4` to deselect it. `Throttle POV Up` and `Down` can be used to scroll.

### In Station

The In Flight UI Navigation remains the same in station provided you haven't connected to the Station interface. Once in the station interface use `Up` and `Down` on the `Throttle POV Hat` to move up and down menus, and `Throttle Btn 1` to select items. `shift` + `Left` and `Right` on `Throttle POV Hat` can be used for moving between sub-panels and selecting cargo amounts. `shift` + `Throttle Btn 4` can be used to exit the current menu.

> **Tip:** You may find it easier to simply use the mouse in station.

### Galaxy Map

A number of overrides are provided for navigating the Galaxy Map. These are:

Axis/Button           | Action
--------------------- | ------
`Stick x`             | _Yaw Camera Left/Right_
`Stick y`             | _Pitch Camera Up/Down_
`Throttle x`          | _Translate Camera Forwards/Backwards_
`Throttle y`          | _Translate Camera Left/Right_
`Throttle Hat 1 Up`   | _Zoom Out_
`Throttle Hat 1 Down` | _Zoom In_
`Throttle Hat 1 Left` | _Galaxy Cam Set Y-Axis to Z-Axis_
`Throttle Hat 3 Up`   | _Translate Camera Up_
`Throttle Hat 3 Down` | _Translate Camera Down_

> **Tip:** It's generally easier to just use the mouse in the Galaxy Map.

### Development Camera

You 'fly' the camera much like you do your ship. Controls are:

Axis/Button             | Action
----------------------- | ------
`Stick x`               | _Roll Camera Left/Right_
`Stick y`               | _Pitch Camera Up/Down_
`Throttle x`            | _Translate Camera Left/Right_
`Throttle y`            | _Translate Camera Up/Down_
`Throttle z`            | _Zoom Camera In/Out_<sup>[1]</sup>
`Stick Hat 3 Forwards`  | _Zoom Camera In_<sup>[1]</sup>
`Stick Hat 3 Backwards` | _Zoom Camera Out_<sup>[1]</sup>
`Stick Hat 3 Left`      | _Yaw Camera Left_
`Stick Hat 3 Right`     | _Yaw Camera Right_

Notes:
> <sup>[1]</sup> To avoid sudden changes in speed when exiting the camera it's best to use `Stick Hat 3` for zoom<br/>

## Landing Overrides

This set up doesn't make use of _Landing Overrides_.

## Joystick Modes

This set up doesn't make use of Joystick modes. The colour of the lit LED on both the `Stick` and the `Throttle` is irrelevant.

## Adding Rudder Pedals

I no longer own the CH Products [Pro Pedals][], however, I have had experience using them. You can add them to this map by clicking the `Add Device` button and selecting the pedals from the list. Order is important in Joystick maps so ensure they are the **3rd** tab, otherwise the CMS script will need to be updated with the new position for the Throttle.

The Axis `Slider 0` and `Slider 1` should be available to bind the yaw axis to, you can then map this in game. The toe pedals can be converted to buttons by using the UI.

> **Note:** If you want to use CMS scripts for your pedals please see [these notes][notes].

## Possible Future Enhancement

With the addition of the new modifier button there are now many duplicate bindings that can be used to map new controls too. The underlying CMS scripts and buttons assignments have been written to be easily expandable. This allows for 33 usable buttons and one POV hat giving a total of 144 button bindings and 8 POV directions. Radical future changes are therefore unlikely.

  * If we end up with an Iron Man mode and an eject button this may get mapped to `shift` + `alt` + `Throttle Hat 1 Down`
  * _Increase_/_Decrease Throttle_ may get mapped to `shift` + `Stick Hat 3 Forwards`/`Backwards` to allow for single hand flying while typing.
  * The _Yaw/Roll Button_ may get replaced with a button that actually swaps `Stick x` for a _Yaw_ axis, and then remaps _Yaw Left_/_Right_ to _Roll Left_/_Right_.
  * For technical reasons I want to look at changing _Stick Hat 3_ to using axis rather than buttons.

## About The Author

This was all put together by [Cmdr Davis][]. There's also a [blog][] and [YouTube][] videos relating to [Elite: Dangerous][]. If you see me in game, say "Hi".

## Misc

I found the template I use for printing my joystick cheat sheets years ago on the internet but I've completely forgotten where from. If you can steer my in the correct direction so I can credit the original author I'd greatly appreciate it. 

## Caveat Emptor

With the exception of the PDF all the files contained in this project are text files so, in theory, nothing bad can happen to your system. That said, you're messing about with game config files so if you break anything, you get to keep both halves. If in doubt always back up.

## Changelog

### Version 2.0.0

  * New `alt` modifier button added
  * All in game controls either have a button, keyboard or axis mapping
  * Moved all fire actions to the trigger (`Stick Btn 1`)
  * Moved all countermeasure actions to `Stick Btn 3`
  * Added new power presets
  * Moved _Silent Running_ to `shift` + `alt` + `Stick Btn 2`
  * Moved _Reset Head-Look_ and _Toggle Dev Camera_ to the `Stick POV Hat`
  * `Stick z` now mapped to _Scanner Range_
  * `Throttle Btn 4` now handles UI Input, UI Back and `ESC`
  * `Throttle POV Hat` now handles all UI movement
  * `Throttle Hat 2` now handled all UI panels and maps
  * Added more functions to `Throttle Hat 1`
  * Wingman functions moved to `Throttle Hat 3`
  * No longer use `Throttle Btn 1`
  * Entire map is now virtual
  * Complete rewrite of the README

### Version 1.2.1

  * Remove mouse axis from head-look so mouse head-look off is now honoured

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

[pdf]: https://github.com/domdavis/ch-products-elite-map/blob/master/layout.pdf?raw=true
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
[notes]: https://github.com/domdavis/ch-products-elite-map/wiki
