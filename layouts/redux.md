# Elite: Dangerous - Full HOTAS layout (version 2.1.0)

This map is a simplified version of the _full_ map and utilises only a single `shift` button. Notes are included below to indicate changes from previous maps. It is also recommended you study the [Layout][pdf] before flying with this map. 

> **Note:** This map uses CMS scripts to maintain compatibility with the _full_ map. If this was built as a stand alone map it could be mapped purely in the UI without scripting.

## Axis Layout

### Fighterstick

Axis      | Action
--------- | ------
`Stick x` | _Roll left/right_
`Stick y` | _Pitch up/down_
`Stick z` | _Scanner Range_<sup>[1]</sup>

Notes:
> <sup>[1]</sup> Previously `Stick z` disabled and enabled `Throttle z`. `Throttle z` cannot be disabled in this map.

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

### Fighterstick

#### Buttons

Button                | Action                     | `shift` Action
--------------------- | -------------------------- | --------------
`Btn 1`               | _Primary Fire_             | _Secondary Fire_
`Btn 2`               | _Toggle Hard Points_       | _Toggle Silent Running_
`Btn 3`<sup>[1]</sup> | _Primary + Secondary Fire_ | _Primary + Secondary Fire_


Notes:
> <sup>[1]</sup> Unlike the _full_ map, countermeasures are on the `Throttle`


### Head-Look (`POV Hat`)

`Stick POV` is used to control head-look with the 8 directions corresponding to the relevant direction to look in. Head-Look is now always on (and mouse head-look is disabled). `Stick POV` also has some modified button assignments<sup>[1]</sup>. These are:

Direction | Action       | `shift` Action
--------- | ------------ | --------------
`Up`      | _Look Up_    | _Reset Head-Look_<sup>[2]</sup>
`Down`    | _Look Down_  | _Toggle Head-Look_
`Left`    | _Look Left_  | _Screen Shot_
`Right`   | _Look Right_ | _High ResolutionScreen Shot_

Notes:
> <sup>[1]</sup> All other combinations are mapped to the 8 directions corresponding to the relevant direction to look in<br/>
> <sup>[2]</sup> Moved from `shift`+`Stick Btn 2` (and `Stick Btn 3` before that)<br/>

#### Power Management (`Hat 1`)

Direction | Action                       | `shift` Action
--------- | ---------------------------- | --------------
`Left`    | _Divert Power to Systems_    | `Preset: Systems`
`Up`      | _Divert Power to Engines_    | `Preset: Engines`
`Right`   | _Divert Power to Weapons_    | `Preset: Weapons`
`Down`    | _Balance Power Distribution_ | `Preset: Misc`<sup>[1],[2]</sup>


Notes:
> <sup>[1]</sup> New preset added in this version<br/>
> <sup>[2]</sup> _Toggle Silent Running_ has moved to `shift`+`Stick Btn 2`<br/>

The presets configure the ship in the following fashion:

Preset              | Systems  | Engines  | Weapons
------------------- | -------- | -------- | -------
`Preset: Systems`   | 4 Pips   | 2 Pips   | 0 Pips
`Preset: Engines`   | 2 Pips   | 4 Pips   | 0 Pips
`Preset: Weapons`   | 0 Pips   | 2 Pips   | 4 Pips
`Preset: Misc`      | 1.5 Pips | 3 Pips   | 1.5 Pips

> **Note:** The presets work by balancing power distribution, then diverting the power as need be. This is literally done by sending the correct key presses in quick succession and so takes a fraction of a second to take effect. You will also notice the visual and audio feedback from the power management panel as the macro runs.

#### Targeting (`Hat 2`)

Direction | Action                         | `shift` Action
--------- | ------------------------------ | --------------
`Up`      | _Select Target Ahead_          | _Select Next Subsystem_
`Down`    | _Select Highest Threat_        | _Select Previous Subsystem_
`Left`    | _Select Previous Hostile Ship_ | _Select Previous Ship_
`Right`   | _Select Next Hostile Ship_     | _Select Next Ship_

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

Button  | Action                                | `shift` Action
------- | ------------------------------------- | --------------
`Btn 1` | _Jettison All Cargo_                  | _Jettison All Cargo_ 
`Btn 2` | _Disable Flight Assist_<sup>[1]</sup> | _Disable Flight Assist_ 
`Btn 3` | _Fire Chaff_<sup>[2]</sup>            | `ESC`
`Btn 4` | _UI Select_                           | _UI Back_

Notes:
> <sup>[1]</sup> Will disable flight assist as long as it's held<br/>
> <sup>[2]</sup> _Galaxy Map_ is now `shift` + `Throttle Hat 2 Left`<br/>

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

Direction | Action                | `shift` Action
--------- | --------------------- | --------------
`Up`      | _Reverse Throttle_    | _Toggle Hyperdrive_
`Down`    | _Boost_               | _Toggle Supercruise_
`Left`    | _Previous Fire Group_ | _Deploy Heat Sink_<sup>[1]</sup>
`Right`   | _Next Fire Group_     | _Use Shield Cell_<sup>[2]</sup>

Notes:
> <sup>[1]</sup> Previously `shift` + `Throttle Hat 3 Left`<br/>
> <sup>[2]</sup> Previously `shift` + `Throttle Hat 3 Right`<br/>

#### UI Panels/Maps (`Hat 2`)

> **Tip:** This hat is mainly used to select a panel to interact with before using the POV hat to then navigate through that panel. Pressing `Up` has the effect of dismissing a panel if one is shown, or giving a slightly wider field of view if no panel is selected. This can be useful for seeing some HUD elements if they're cut off by the edge of the screen.

> **Tip:** Selecting a direction a second time will also dismiss the currently displayed panel.

Direction | Action          | `shift` Action
--------- | ----------------| -----------------------------
`Up`      | _UI Focus Mode_ | _Comms Panel_<sup>[1]</sup>
`Down`    | _Radar Panel_   | _Next system In Route_
`Left`    | _Target Panel_  | _Galaxy Map_<sup>[2]</sup>
`Right`   | _Systems Panel_ | _System Map_

Notes:
> <sup>[1]</sup> By default the text entry box is not selected. Select it using `Btn 4`. Deselect it by using `shift` + `alt` + `Btn 3`<br/>
> <sup>[2]</sup> Previously `Throttle Btn 3` (and `shift` + `Throttle Btn 3` prior to that)<br/>

#### Wingmen, Landing Gear and Cargo (`Hat 3`)

Direction | Action                           | `shift` Action
--------- | -------------------------------- | -----------------------------
`Left`    | _Select Wingman 1_<sup>[1]</sup> | _Select Wingman 1_
`Up`      | _Select Wingman 2_<sup>[2]</sup> | _Wingman Nav-Lock_<sup>[4]</sup>
`Right`   | _Select Wingman 3_<sup>[3]</sup> | _Select Wingman 3_
`Down`    | _Toggle Landing Gear_            | _Toggle Cargo Scoop_

Notes:
> <sup>[1]</sup> Previously `shift` + `Throttle POV Left`<br/>
> <sup>[2]</sup> Previously `shift` + `Throttle POV Up`<br/>
> <sup>[3]</sup> Previously `shift` + `Throttle POV Right`<br/>
> <sup>[4]</sup> PReviously `shift` + `Throttle POV Down`<br/>

### Mouse

The left mouse button acts like UI Select when the mouse cursor is over a button.

## Keys

Pressing `SPACE` brings up Quick Comms, i.e. a chat entry to the current target. This isn't mapped to a joystick button currently as you'll need to use the keyboard anyway to enter text.

## Navigating The UI

### In Flight

UI Navigation is a little counter intuitive if you simply go by button assignments. In flight you generally use `Throttle Hat 2` and either `Left` or `Right` to select the relevant UI Panel. `Throttle POV` is then used to navigate between tabs and up and down within tabs with `Throttle Btn 4` used to select elements. `shift` + `Throttle POV Left` and `Right` can then be used to alter values that can be altered (for example system priority) and to move between sub-panels (e.g. the _Location_ list and map buttons on the _Navigation_ tab, and _Fire Groups_ in the _Fire Groups_ tab).

> **Tip:** It is also possible to bring up the relevant UI panels with Head Look by looking in the right direction.

### Comms Menu

Use `Left` and `Right` on the `Throttle POV Hat` to navigate the _Comms Menu_. Use `Throttle Btn 4` to select an action. If the _Text Input_ box is selected then use `shift` + `Throttle Btn 3` to deselect it. `Throttle POV Up` and `Down` can be used to scroll.

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

[pdf]: redux.pdf