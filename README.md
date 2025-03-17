Original game modified to to suit the needs of a small treasure hunt style event.</br>
Done on behalf of KIIT Electrical Society, for KIIT Fest Day 3 (16.02.25).

The game was supposed to lock progress to the next stage until the required answer was discovered. This answer was supposed to be found out from a physical tresure hunt activity. The game has been modified in the following way

- Removed the footer and survey button at index.html
- Change the title in html
- Hide the About, Freeplay, and Settings buttons from the game main screen
- Moved around the buttons a bit on the main screen
- Remove the replay level button from stage ends
- Remove the "by TAUM" in spritesheetmenu.json ()
- Clamp min and max levels to 14 and 18 (this, by extension, skips the tutorials)

- Make the hint button invisible in Menu.prototype.fadeInHintBtn() by adding this line -> this.makeHintBtnInvisible();

- Added new function showPasswordPopup() to menu.js. which is instantiated by gamestate.
- Gamestate then calls it to show a password popup before forwarding to next level.

- Passwords, hints and popups are all handled in menu.js
- Passwords are SHA256 hashed and store client side


//might add more details later
