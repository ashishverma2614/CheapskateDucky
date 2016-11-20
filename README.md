# CheapskateDucky
Project inspired by USB Rubber Ducky ( http://usbrubberducky.com )

This code reads from sd card and then reproduces file content as keyboard events.

Used Arduino must be 32u4 based to have keyboard interface support.

Unless escape sequences are used each line of configured input file (test.txt) is
  used as input that is inserted through key presses. Escape sequences may be used
  to press special keys or key combinations.

  Sequences:
  - To simulate pressing left Crtl, left Alt and t -buttons simultaneously use sequence [128+130+116]
  - To add 1000ms delay use sequence [DEL1000]
  - To actually use [ or \ character as input escape it with backslash. \[
  - Key codes may be found from Arduino reference: <https://www.arduino.cc/en/Reference/KeyboardModifiers> or from any ascii table (e.g. <http://www.asciitable.com/> )
