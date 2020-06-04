/* 
 *  MIDI Footswitch
   You must select MIDI from the "Tools > USB Type" menu
   To view the raw MIDI data on Linux: aseqdump -p "Teensy MIDI"
*/

#include <Bounce.h>
#define BUTTON_DEBOUNCE 50 // 50 = 50 ms debounce time

// the MIDI channel number to send messages
const int channel = 2;

Bounce button5 = Bounce(5, BUTTON_DEBOUNCE);
Bounce button6 = Bounce(6, BUTTON_DEBOUNCE);  
Bounce button7 = Bounce(7, BUTTON_DEBOUNCE);  
Bounce button8 = Bounce(8, BUTTON_DEBOUNCE);  
Bounce button9 = Bounce(9, BUTTON_DEBOUNCE);
Bounce button10 = Bounce(10, BUTTON_DEBOUNCE);  
Bounce button14 = Bounce(14, BUTTON_DEBOUNCE); 
Bounce button15 = Bounce(15, BUTTON_DEBOUNCE); 
Bounce button16 = Bounce(16, BUTTON_DEBOUNCE);
Bounce button17 = Bounce(17, BUTTON_DEBOUNCE);
Bounce button18 = Bounce(18, BUTTON_DEBOUNCE);
Bounce button19 = Bounce(19, BUTTON_DEBOUNCE);
Bounce button20 = Bounce(20, BUTTON_DEBOUNCE);

void setup() {
  // Configure the pins for footswitch buttons as input mode = pullup resistors.
  // The pushbuttons connect from each pin to ground.  When
  // the button is pressed, the pin reads LOW because the button
  // shorts it to ground.  When released, the pin reads HIGH
  // because the pullup resistor connects to +5 volts inside
  // the chip. 
  // Teensy++ 2.0 LED, may need 1k resistor pullup

  pinMode(5, INPUT_PULLUP);
  pinMode(6, INPUT_PULLUP);
  pinMode(7, INPUT_PULLUP);
  pinMode(8, INPUT_PULLUP);
  pinMode(9, INPUT_PULLUP);
  pinMode(10, INPUT_PULLUP);
  pinMode(14, INPUT_PULLUP);
  pinMode(15, INPUT_PULLUP);
  pinMode(16, INPUT_PULLUP);
  pinMode(17, INPUT_PULLUP);
  pinMode(18, INPUT_PULLUP);
  pinMode(19, INPUT_PULLUP);
  pinMode(20, INPUT_PULLUP);
}

void loop() {
  // Get a reading from the button
  button5.update();
  button6.update();
  button7.update();
  button8.update();
  button9.update();
  button10.update();
  button14.update();
  button15.update();
  button16.update();
  button17.update();
  button18.update();
  button19.update();
  button20.update();


  // Turn notes on if a button has been connected to ground
  if (button5.fallingEdge()) {
    usbMIDI.sendNoteOn(60, 99, channel);  // 60 = C4
  }
  if (button6.fallingEdge()) {
    usbMIDI.sendNoteOn(61, 99, channel);  // 61 = C#4
  }
  if (button7.fallingEdge()) {
    usbMIDI.sendNoteOn(62, 99, channel);  // 62 = D4
  }
  if (button8.fallingEdge()) {
    usbMIDI.sendNoteOn(63, 99, channel);  // 63 = D#4
  }
  if (button9.fallingEdge()) {
    usbMIDI.sendNoteOn(64, 99, channel);  // 64 = E4
  }
  if (button10.fallingEdge()) {
    usbMIDI.sendNoteOn(65, 99, channel);  // 65 = F4
  }
  if (button14.fallingEdge()) {
    usbMIDI.sendNoteOn(66, 99, channel);  // 66 = F#4
  }
  if (button15.fallingEdge()) {
    usbMIDI.sendNoteOn(67, 99, channel);  // 67 = G4
  }
  if (button16.fallingEdge()) {
    usbMIDI.sendNoteOn(68, 99, channel);  // 68 = G#4
  }
  if (button17.fallingEdge()) {
    usbMIDI.sendNoteOn(69, 99, channel);  // 69 = A5
  }
  if (button18.fallingEdge()) {
    usbMIDI.sendNoteOn(70, 99, channel);  // 70 = A#5
  }
  if (button19.fallingEdge()) {
    usbMIDI.sendNoteOn(71, 99, channel);  // 71 = B5
  }
  if (button20.fallingEdge()) {
    usbMIDI.sendNoteOn(72, 99, channel);  // 72 = C6
  }


  // Turn notes off if a button was disconnected from ground
  if (button5.risingEdge()) {
    usbMIDI.sendNoteOff(60, 0, channel);  // 60 = C4
  }
  if (button6.risingEdge()) {
    usbMIDI.sendNoteOff(61, 0, channel);  // 61 = C#4
  }
  if (button7.risingEdge()) {
    usbMIDI.sendNoteOff(62, 0, channel);  // 62 = D4
  }
  if (button8.risingEdge()) {
    usbMIDI.sendNoteOff(63, 0, channel);  // 63 = D#4
  }
  if (button9.risingEdge()) {
    usbMIDI.sendNoteOff(64, 0, channel);  // 64 = E4
  }
  if (button10.risingEdge()) {
    usbMIDI.sendNoteOff(65, 0, channel);  // 65 = F4
  }
  if (button14.risingEdge()) {
    usbMIDI.sendNoteOff(66, 0, channel);  // 66 = F#4
  }
  if (button15.risingEdge()) {
    usbMIDI.sendNoteOff(67, 0, channel);  // 67 = G4
  }
  if (button16.risingEdge()) {
    usbMIDI.sendNoteOff(68, 0, channel);  // 68 = G#4
  }
  if (button17.risingEdge()) {
    usbMIDI.sendNoteOff(69, 0, channel);  // 69 = A5
  }
  if (button18.risingEdge()) {
    usbMIDI.sendNoteOff(70, 0, channel);  // 70 = A#5
  }
  if (button19.risingEdge()) {
    usbMIDI.sendNoteOff(71, 0, channel);  // 71 = B5
  }
  if (button20.risingEdge()) {
    usbMIDI.sendNoteOff(72, 0, channel);  // 71 = C6
  }
}
  
  


 
