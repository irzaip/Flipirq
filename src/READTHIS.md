======  Make arduino midi controller ======


referensi: 
  *[[https://www.youtube.com/watch?v=Nkxh29YNNmA]]
  *[[https://www.arduino.cc/en/Hacking/DFUProgramming8U2]]
           
perlu : 
  *[[https://www.microchip.com/Developmenttools/ProductDetails/FLIP]]
        
        
* Install FLIP.
Apabila mau connect ada error.

Solution - Flip error "AtLibUsbDfu.dll not found" when flashing Arduino
  *[[https://www.youtube.com/watch?v=KQ9BjKjGnIc]]

Pastikan ter-deteksi arduino di Device manager.
Gunakan driver dari directory installasi FLIP

Kalau buat arduino UNO. gunakan **ATmega16U2**

Cara Flash dgn FLIP:
  *[[https://www.youtube.com/watch?v=Nkxh29YNNmA&feature=emb_logo]]
  * klik target device ATmega16U2 atau ATmega32U4
  * Select communication medium ⇒ USB
  * Klik Load Hex FILE  => dart midi / flipper / yg lain.
  * Klik reset arduino dengan short jumper.
  * Pastikan program sudah set serial di baud rate   **Serial.begin(31250);**

Itu kalau mau jadi midi USB.
Kalau tidak mau jadi USB Midi. gunakan.
  * Hairless MidiSerial [[https://projectgus.github.io/hairless-midiserial/]] 
  * LoopMidi [[http://www.tobias-erichsen.de/software/loopmidi.html]]

Kalau ingin bisa USB Midi Arduino uno ada MocoLuca
  * [[https://github.com/kuwatay/mocolufa]]
  * [[http://morecatlab.akiba.coocan.jp/lab/index.php/aruino/midi-firmware-for-arduino-uno-moco/?lang=en]]
  * [[https://www.youtube.com/watch?v=18OKo9sQ_s0&t=186s]]
  * [[https://moco-lufa-web-client.herokuapp.com/#/]]  ⇐⇐ ✔

referensi library Midi Usb di Arduino:

  * [[https://github.com/FortySevenEffects/arduino_midi_library]] - untuk Uno ATmega16U2
  * [[https://github.com/lathoub/Arduino-USBMIDI]] - untuk pro, micro pro, dll ATmega32U4

Referensi program flipper original:
  * [[https://www.musiconerd.com/projects]]
