# Process and Documentation

## Photographs



## Video

## Code 

- void setup() {
  - // Pins 2 and 3 are connected to In1 and In2 respectively
  - // of the L298 motor driver
  - pinMode(2, OUTPUT);
  - pinMode(3, OUTPUT);
}

- void loop() {
 -  // make the motor turn in one direction
  - digitalWrite(2, LOW);
  - analogWrite(3, 195); // go fast
  - delay(5000); // let it turn for 5 seconds

  - // digitalWrite(2, LOW);
  - analogWrite(3, 230); // faster!
  - delay(8000); // let it turn for 5 seconds

  - // now reverse direction
  - digitalWrite(2, HIGH);
  - analogWrite(3, 50); // this will be fast
  - delay(5000);

  - analogWrite(3, 100); // slower
  - delay(8000);
}
