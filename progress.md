more to come, this is just my notes right now

done
==
- purchased MSA Advantage 1000 (used, ebay)
- purchased outsert for MSA Advantage (used, ebay)
  - make sure to order matching outsert size for your mask!! (check the markings at the top of the mask's visor
  - undyed alone is much cheaper than premade ($20ish vs $60ish), but conceptually it's only slightly cheaper to buy an undyed + fabric dye + a big pot from a thrift store (estimated $50). if shipping fees/tax kill it in your area, consider dying it yourself, but otherwise from an ecological perspective it probably makes more sense to buy the pre-dyed one
  - if you dye it yourself, make sure **you never use the pot in question for food afterwards**; fabric dye is not foodsafe and will likely leech into anything you cook in this pot afterwards
- [purchased one-way film](https://www.amazon.com/dp/B07ZGCBZZT?psc=1)
- [purchased LED strip for mask](https://www.amazon.com/KWMSTPLT-Individually-Addressable-Programmable-Non-Waterproof/dp/B09P8MH56K)
- [purchased mp3 player module](https://www.amazon.com/gp/product/B0CF593SWY?psc=1) (which, misleading name aside, should just be an SD card slot & an audio jack + DAC)


plan of action
==
- one-way film along inside of visor outsert
- RGB strips along inside of visor outsert
- some kind of microcontroller (esp32?)
- microcontroller + battery on wristband
- wii nunchuck in hand, connected to microcontroller
- audio jack on microcontroller
- SD card with hypnofiles on the serial mp3 player
- 3d print case for electronics

todo
==
- we're gonna need to follow a collection of tutorials here
  - ~~[RGB strip via ESP32](https://randomnerdtutorials.com/esp32-esp8266-rgb-led-strip-web-server/)~~
      - Not that tutorial, thats for non-addressable RGB
      - Try this one https://www.electronicsforu.com/electronics-projects/diy-wireless-addressable-rgb-controller
      - Or maybe https://esp32io.com/tutorials/esp32-ws2812b-led-strip
      - [ACTUALLY TRY THIS ONE FIRST](https://www.programmingboss.com/2023/07/control-ws2812b-addressable-5050-RGB-LED-Strip-Using-ESP32-Adafruit-NeoPixel-library.html) allegedly this uses an adafruit library == easy for my inexperienced ass to follow
  - for hypnofiles, [part of this tutorial for ESP32 Audio player](https://esp32io.com/tutorials/esp32-audio), which should be most of it, but you'll have to figure *something* out for the volume (and also why its not putting any sound out)
  - [spirals on visor](https://www.techwalla.com/articles/how-to-make-spirals-in-gimp)
  - [ESP32 and nunchuck](https://github.com/moefh/esp32-wii-nunchuk)
- you'd better cite your sources young gamer
- gotta fix the 3d printer first lolol
- when writing the code, function to convert an image -> ~~13x7 dots? maybe have checks to see if res is 13x7 already~~ looks more like 
- confirm the actual resolution
- need to make a new strap- documentation is being written, just need to sew

explore
==
- it'd be very funny to have a shittly encoded [movie on the drone mask](https://www.instructables.com/Play-Video-With-ESP32/), and then to plug in speakers. will need to reencode the videos with FFMPEG ahead of time, in the appropriate resolution (13x7?). audio quality can still be ok
- buy a nosecup? will help much with fogging allegedly
- [Integrate a Pizeo buzzer!](https://esp32io.com/tutorials/esp32-piezo-buzzer) This will allow the drone to beep!
- Host a webserver & AP on the esp32! This will let a dominant connect to the mask and remotely control it
- Have some kind of display pointing back at the drone for spirals
