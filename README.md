Original game modified to to suit the needs of a small treasure hunt style event.</br>
Done on behalf of KIIT Electrical Society, for KIIT Fest Day 3 (16.02.25).

The game was supposed to lock progress to the next stage until the required answer was discovered. This answer was supposed to be found out from a physical tresure hunt activity. The game has been modified in the following way

- Removed the footer and survey button at index.html
- Change the title in html
- Hide the About, Freeplay, and Settings buttons from the game main screen
- Moved around the buttons a bit on the main screen
- Remove the replay level button from stage ends
- Remove the "by TAUM" in spritesheetmenu.json ()
- Clamp min and max levels between 14 and 18 (this, by extension, skips the tutorials)

- Make the hint button invisible in Menu.prototype.fadeInHintBtn() by adding this line -> this.makeHintBtnInvisible();

- Added new function showPasswordPopup() to menu.js. which is instantiated by gamestate.
- Gamestate then calls it to show a password popup before forwarding to next level.

- Passwords, hints and popups are all handled in menu.js
- Passwords are SHA256 hashed and store client side

## As it looks now
<table>
  <tr>
    <td><image src="https://github.com/user-attachments/assets/8cc03730-8cc7-400d-985b-0bdd35cc7873"></td>
    <td>
      <image src="https://github.com/user-attachments/assets/07d866e4-a382-4ea9-8236-d6c6147afe53">
    </td>
  </tr>

        
  <tr>
    <td><image src="https://github.com/user-attachments/assets/04c2b7a4-4672-47e9-9982-2b16f83c72fd"></td>
    <td>
      <image src="https://github.com/user-attachments/assets/823bdbc9-6140-43d9-9b8a-eddbb17856fb">
    </td>
  </tr>

        
  <tr>
    <td><image src="https://github.com/user-attachments/assets/0bcc6350-8d2e-40ed-9df0-606f816dd835"></td>
    <td>
      <image src="https://github.com/user-attachments/assets/1a52620c-8e98-4a4a-8a4f-7f2ae9e8c0a0"></td>
  </tr>

  <tr>
    <td>
      <image src="https://github.com/user-attachments/assets/e2c12f52-2318-4a39-917a-37065ed63625"></td>
  </tr>

        
</table>

## Currently set passwords
- [Hint A] `frequency`
- [Hint B] `inductance`
- [Hint C] `generator`
- [Hint D] `electricvehicle`
- [Hint E] `transmission`


## Footnote
The project removes the name of the authors from the deployment, not with an intention to steal credit. The idea was to prevent players from realizing that this is an openly available game on the internet, as that might have encouraged them to look for walkthroughs.
