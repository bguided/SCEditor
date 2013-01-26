---
layout: release
title: Version 1.4.1 released
excerpt: Details of the 1.4.1 release
tags: [releases, 1.4.1]
categories:
    - releases
---
## Version 1.4.1

Version 1.4.1 has been released with numerous bug fixes. Thanks to everyone who contributed!

Other than bug fixes the main changes are plugin support, the `blur()`, `keyDown()`, `keyPress()`, `keyUp()`, `rtl()` and `maximize()` methods and RTL theme support.

**Important** The minified file `jquery.sceditor.min.js` no longer has the BBCode plugin bundled in it. For both the editor and BBCode plugin use the `jquery.sceditor.bbcode.min.js` file instead.

### Full 1.4.1 changelog:

 * Dropped GPL to match jQuery license.  
     The editor can still be used under the GPLv2, GPLv3 or any other MIT compatible  
     license. Changes can't be submitted back unless they are licensed under the MIT  
     but then they couldn't before either as it was dual licensed under the MTI so  
     really there isn't any change, just a bit simpler.
 * Added blur, keyDown, keyPress and KeyUp helpers
 * Added Turkish translation  
     - Thanks to @MYaman34 for translating.
 * Added button state support
 * Added better plugin system
 * Fixed emoticons now showing their code as a tooltip.
 * Added support for custom emoticon tooltips.  
     - Thanks to @Spuds for reporting
 * Added nodechanged event.
 * Improved BBCode attribute quoting support.  
     - Thanks to @Spuds for reporting
 * Added Arabic translation.  
     - Thanks to @Atramez-Zeton for translating
 * Added disablePasting option.
 * Fixed problem with HTML5 form validation not working when using the editor.  
     The editor will now just remove the required attribute from the original textarea  
     so validation will either need to be done server side or manually.
 * Added tabindex support. The tabindex will be picked up from the original textarea.  
     - Thanks to @bmxgrover for reporting  
     - Thanks to @Spuds for reporting
 * Fixed bug with nested lists.  
     - Thanks to @brunoais for reporting.
 * Improved IE resize speed.
 * Update themes to support showing active commands.
 * Update themes to support showing a commands icon, text or both.
 * Added new Monocon icons, licensed under the MIT license.
 * Added selectionchanged event
 * Fixed bug with LTR command not working.  
     - Thanks to @charafweb for reporting
 * Added zIndex option to allow setting the containers z-index.  
     Fixes bug with modal jQuery UI dialogs.  
     - Thanks to @prdatur for reporting and the fix.
 * Fixed bug with percentage based widths.  
     - Thanks to @charafweb for reporting.
 * Improved RTL support. Added rtl() helper and improved all themes RTL support.
 * Added maximize command and maximize() helper.
 * Fixed bug with sentences wrapped in [] sometimes causing problems.
 * 	- Thanks to @liamdawe for reporting
