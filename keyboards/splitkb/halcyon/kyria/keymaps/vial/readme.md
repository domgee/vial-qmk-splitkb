1. Make this repo qmk home, from root: `qmk setup -H $(realpath .)` 
2. From https://github.com/splitkb/qmk_userspace
    - copy keyboards/splitkb/halcyon/kyria/keymaps/vial_hlc to this repo, keyboards/splitkb/halcyon/kyria/keymaps/vial
    - copy users/halcyon_modules to this repo, users/halcyon_modules
3. Convert keymap.json to .c: `qmk json2c keymap.json > keymap.c`
4. Build: `make clean; make splitkb/halcyon/kyria/rev4:vial -e HLC_NONE=1`

https://docs.splitkb.com/product-guides/halcyon-series/advanced/compiling-firmware
https://get.vial.today/docs/porting-to-vial.html
https://docs.qmk.fm/features/rgb_matrix
