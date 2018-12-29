## Changelog

### Version 3.1.0

  * Use different keybindings to avoid clashes on concurrent button presses
  * Add playlist controls in place of screen shot controls.
  * Provided a link for donations (one can always dream ;) )

### Version 3.0.0

Complete rebuild of the map from the ground up.

  * Single, unified map
  * Drop mappings not required in VR
  * Easier integration with Voice Attack through use of keys rather than buttons
  * Add new bindings for Elite:Dangerous 3.3

### Version 2.1.1

  * Added binding to show CQC scores

### Version 2.1.0

This change simply adds the _redux_ version of the map. No changes have been
made to the _full_ map other than the location of the files and some fixes to
the description.

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
    _Fire Heat Sync_ on the `Stick` and now lives with  _Use Shield Cell_ on the
     `Throttle`
  * Minor tweaks to axis direction in the _Galaxy Map_
  * Minor tweaks to the way headlook works with the mouse and bindings
  * Added changelog :)
