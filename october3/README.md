# Process and Documentation

## Photographs

![1](https://github.com/shamsasaeed/Preforming-Robots/blob/main/1.jpg)

![2](https://github.com/shamsasaeed/Preforming-Robots/blob/main/2.jpg)

![3](https://github.com/shamsasaeed/Preforming-Robots/blob/main/3.jpg)

## Video

Video will be taken in class

## Code 

- void setup() {
 -  // Pins 2, 3, 4, 5 are connected to In1 In2 In3 In4 respectively
-   // of the L298 motor driver
 -  pinMode(2, OUTPUT);
 -  pinMode(3, OUTPUT);
 -  pinMode(4, OUTPUT);
  - pinMode(5, OUTPUT);
}

- void loop() {

 -  // make the motors turn in one direction
  - digitalWrite(2, LOW);
  - digitalWrite(5, LOW);
 -  analogWrite(3, 100); // go fast
  - analogWrite(4, 100);
 -  delay(3000); // let it turn for 3 seconds

  - // going on one direction
  - digitalWrite(2, HIGH);
  - //digitalWrite(5, HIGH);
  - analogWrite(3, 140); // this will be slower
  - //analogWrite(4, 50);
  - delay(4000); // turn for 4 secs

- // reverse direction
 -  digitalWrite(2, HIGH);
 -  digitalWrite(5, HIGH);
 -  analogWrite(3, 210); // this will be slower
 -  analogWrite(4, 210);
  - delay(4000);

  - analogWrite(3, 100); // slower
 -  analogWrite(4, 100);
  - delay(3000);


}

