# Iris Keymaps

## Process

This process must be performed for both halves of   

### Configurating the Keymap

Create a new keymap. This can either be done:
    - via the [qmk configurator](https://config.qmk.fm/#/keebio/iris/rev4/LAYOUT)
    - via the qmk cli `qmk new-keymap` (note that there are [prerequisites to configure qmk](https://docs.qmk.fm/newbs_building_firmware))
    
Sanity check that it compiles by using `qmk compile -kb <keyboard> -km <keymap>`.

### Flashing the Keymap

Once the keymap is created you can flash it to the board. 
All of these steps must be done twice - once on each side of the board. 

1. Remove the back plate from the board
1. Connect one half of the board via USB. 
1. Press the "reset" button on that side of the board 
1. Flash the board with the newly created keymap: `qmk flash -kb <keyboard> -km <keymap>`
1. Repeat for the other half of the board
