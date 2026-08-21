
# Install to keyboard 
```
cd ~
git clone https://github.com/tmrotz/qmk_firmware.git
git submodule
qmk config user.keyboard=crkbd/rev1
qmk config user.keymap=travis
sudo mkdir -p /mnt/e && qmk compile && sleep 5 && sudo mount -t drvfs E: /mnt/e && cp ~/qmk_firmware/crkbd_rev1_travis.uf2 /mnt/e/
```

The first time will require password. You have 5 seconds to then press the QK_BOOT key.

