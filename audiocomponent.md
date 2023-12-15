log for getting audio working

goal for this log is to make the ESP32 read from a microsd card and play audio from the aux out, with intention of listening to a hypnofile (not for actual effect but for just testing)
resources;
- 1x [esp32 wroom](https://www.ebay.com/itm/124835593994)
- 2x [mp3 player module](https://www.amazon.com/dp/B0CF593SWY?psc=1)
- [this tutorial](https://esp32io.com/tutorials/esp32-mp3-player)

1) desolder the pin header on the mp3 module, that'll just get in the way
hmm, seems like the tutorial's esp 32 has 6 more pins than mine- i have a 30 pin esp32, they show a 36 pin esp32
digging into things further the extra 6 pins seem to be directly connected to the flash mem so that shouldnt be an issue
it'd help a lot if this website's rendition of the esp32 actually had markings on the board

ok using my brain (unfortunate, drones hate being mindful), we just need 3.3v/gnd/tx/rx, and my board has markings for that, so letsa go

...ok nice and easy, done, but I realized i have the wrong firmware on the esp32- check flashing.md

2) tbd
