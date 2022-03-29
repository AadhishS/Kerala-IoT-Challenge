---

# Feel free to add content and custom Front Matter to this file.

# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default

---
# Kerala-IoT-Challenge

  <p><strong>Foxlab Makerspace</strong> in association with <strong>GTech - Group of Technology Companies</strong> in Kerala is launching our prestigious program  <strong>“Kerala&nbsp;IoT Challenge 2021”</strong>,  with a vision to mould 100 IoT experts in Kerala, hosting on the µLearn platform. <strong>Kerala IoT Challenge</strong> is a program designed in 4 levels followed by a hackathon to identify and train quality industry leaders in the IoT domain, while any novice learner can start with layer 1 and others can enter laterally to the desired layer after an evaluation.</p>



# <u><b>About Me</b></u>

<blockquote>

Hi, I am  AADHISH S. I am a second year B-Tech Computer Science student  @ <a href="http://mahagurutech.ac.in" target="_blank">Mahaguru&nbsp; Institute&nbsp; of&nbsp; Technology</a>.

I have helped in some computer science and electronics projects. I love to learn new things and I like to be updated with development in the Tech Industry. I am Fascinated  about Tech, Business and related stuff.  

</blockquote>

____
____

# <u><b>LEVEL - 1</b></u>

# <u><b>Experiments</b></u>

### Exp 1 : Hello World LED Blinking

### Hardware Needed:
   * Arduino Uno Board x1
   * USB Cable x1
   * LED (Any Color) x1
   * 220 OHM Resistor X1 
   * Breadboard
   * Jumper Wires (Male to Male ) x2

### Code
    int ledPin = 10; // define digital pin 10.
    void setup()
    {
     pinMode(ledPin, OUTPUT);// define pin with LED connected as output.
    }
    void loop()
    {
     digitalWrite(ledPin, HIGH); // set the LED on.
     delay(1000); // wait for a second.
     digitalWrite(ledPin, LOW); // set the LED off.
     delay(1000); // wait for a second
    }


### Video
<iframe width="600" height="315" src="https://youtu.be/GxmuL_qJiPE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

___
# <u><b>LEVEL - 2</b></u>

# <u><b>Experiments</b></u>
### Exp 2 : Traffic Light

### Hardware required
  * Arduino board x1
  * USB cable x1
  * Red M5 LED x1
  * Yellow M5 LED x1
  * Green M5 LED x1
  * 220Ω resistor x3
  * Breadboard x1
  * Breadboard jumper wires as needed

### Code
    int red =10; // initialize digital pin 8.
    int yellow =7; // initialize digital pin 7.
    int green =4; // initialize digital pin 4.
    void setup()
    {
      pinMode(red, OUTPUT);// set red LED pin as “output”
      pinMode(yellow, OUTPUT); // set yellow LED pin as  “output”
      pinMode(green, OUTPUT); // set green LED pin as “output”
    }
    void loop()
    {
      digitalWrite(green, HIGH);// turn on green LED
      delay(5000);// wait 5 seconds
      digitalWrite(green, LOW); // turn off green LED
      for(int i=0;i<3;i++)// blinks for 3 times
      {
       delay(500);// wait 0.5 second
       digitalWrite(yellow, HIGH);// turn on yellow LED
       delay(500);// wait 0.5 second
       digitalWrite(yellow, LOW);// turn off yellow LED
      } 
      delay(500);// wait 0.5 second
      digitalWrite(red, HIGH);// turn on red LED
      delay(5000);// wait 5 seconds
      digitalWrite(red, LOW);// turn off red LED
    }

### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/-Da8OEcXSas" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# <u><b>LEVEL - 3</b></u>

# <u><b>Experiments</b></u>

### Exp 3 : LED Chasing Effect

### Hardware required
  * LED x6
  * Arduino board x1
  * 220Ω resistor x6
  * Breadboard x1
  * USB cable x1
  * Breadboard wire x13

### Code
    int first= 2;  // the I/O pin for the first LED
    int last= 6;   // number of LEDs
    void setup(){
     for (int i = start; i < first + last; i ++){
      pinMode(i, OUTPUT);   // set I/O pins as output
     }
    }
    void loop(){
     for (int i = BASE; i < start +; i ++){
      digitalWrite(i, LOW);    // set I/O pins as “low”, turn off LEDs one by one.
      delay(200);        // delay
    }
     for (int i = BASE; i < BASE + NUM; i ++){
      digitalWrite(i, HIGH);    // set I/O pins as “high”, turn on LEDs one by one
      delay(200);        // delay
     }  
    }

### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/dLirEbPWCPg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# <u><b>LEVEL - 4</b></u>

# <u><b>Experiments</b></u>

### Exp 4 : Button Controlled LED

### Hardware required
* Arduino Uno
* Button switch*1
* Red M5 LED*1
* 220ΩResistor*1
* 10KΩ Resistor*1
* Breadboard*1
* Breadboard Jumper Wire*6
* USB cable*1

### Code
    int ledpin=11;// initialize pin 11
    int inpin=3;// initialize pin 3
    int val;// define val
    void setup()
    {
    pinMode(ledpin,OUTPUT);// set LED pin as “output”
    pinMode(inpin,INPUT);// set button pin as “input”
    }
    void loop()
    {
    val=digitalRead(inpin);// read the level value of pin 3 and assign if to val
    if(val==LOW)// check if the button is pressed, if yes, turn on the LED
    { digitalWrite(ledpin,LOW);}
    else
    { digitalWrite(ledpin,HIGH);}
    }
### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/xiQ2F2ps62I" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# <u><b>LEVEL - 5</b></u>

# <u><b>Experiments</b></u>


### Exp 5 : Buzzer

### Hardware required
* Arduino Uno
* Buzzer x1
* Breadboard x1
* Breadboard Jumper Wire x2
* USB cable x1

### Code
    int buzzer=8;// initialize digital IO pin that controls the buzzer
    void setup() 
    { 
      pinMode(buzzer,OUTPUT);// set pin mode as “output”
    } 
    void loop() 
    {
    digitalWrite(buzzer, HIGH); // produce sound
    }
### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/QN5DBPFhgCU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
____

# <u><b>LEVEL - 6</b></u>

# <u><b>Experiments</b></u>

### Exp 6 : RGB LED

### Hardware required
* Arduino Uno
* USB Cable x1
* RGB LED x1
* Resistor x3
* Breadboard jumper wire x5

### Code
    int redpin = 11; //select the pin for the red LED
    int bluepin =10; // select the pin for the blue LED
    int greenpin =9;// select the pin for the green LED
    int val;
    void setup() {
      pinMode(redpin, OUTPUT);
      pinMode(bluepin, OUTPUT);
      pinMode(greenpin, OUTPUT);
      Serial.begin(9600);
    }
    void loop() 
    {
    for(val=255; val>0; val--)
      {
      analogWrite(11, val);
      analogWrite(10, 255-val);
      analogWrite(9, 128-val);
      delay(1); 
      }
    for(val=0; val<255; val++)
      {
      analogWrite(11, val);
      analogWrite(10, 255-val);
      analogWrite(9, 128-val);
      delay(1); 
      }
    Serial.println(val, DEC);
    }
### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/CHlVNigktpU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

# <u><b>LEVEL - 7</b></u>

# <u><b>Experiments</b></u>

### Exp 7 : LDR Light Sensor

### Hardware required
* Arduino Uno Board
* Photo Resistorx1
* Red M5 LED x1
* 10KΩ Resistor x1
* 220Ω Resistor x1
* Breadboard x1
* Breadboard Jumper Wire x5
* USB cable x1

### Code
    void setup() {
      pinMode(8,INPUT);
      pinMode(9,OUTPUT);
      Serial.begin(9600); //initialise serial monitor
    }

    void loop() {
      int temp=digitalRead(8);       //assign value of LDR sensor to a temporary variable
      Serial.println("Intensity="); //print on serial monitor using ""
      Serial.println(temp);         //display output on serial monitor
      delay(300);
      if(temp==HIGH)               //HIGH means,light got blocked
      digitalWrite(9,HIGH);        //if light is not present,LED on
      else
      digitalWrite(9,LOW);         //if light is present,LED off
    }

### Video
<iframe width="600" height="315" src="https://www.youtube.com/embed/ae_OpAmNPWU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
____










<h3 id="experiment-8---flame-sensor">Experiment 8 - Flame Sensor</h3>

<h4 id="components-required-4">Components Required</h4>
<ul>
  <li>Arduino Uno Board</li>
  <li>IR Reciever</li>
  <li>LED*1</li>
  <li>10KΩ Resistor*1</li>
  <li>Breadboard*1</li>
  <li>Breadboard Jumper Wire*4</li>
  <li>USB cable*1</li>
</ul>


<h4 id="code-7">Code</h4>
<pre><code class="language-ino">
int flame=0;// select analog pin 0 for the sensor
int LED=9;// select digital pin 9 for the LED
int val=0;
 void setup() 
{
 pinMode(LED,OUTPUT); 
 pinMode(flame,INPUT); 
 Serial.begin(9600);
void loop() 
{ 
  val=analogRead(flame);// read the analog value of the sensor 
  Serial.println(val);// output and display the analog value
  if(val&gt;=600)// when the analog value is larger than 600, the led will glow
  {  
   digitalWrite(LED,HIGH); 
   }else 
   {  
     digitalWrite(LED,LOW); 
    }
   delay(500); 
}
</code></pre>
<h3 id="experiment-9----lm35-temperature-sensor">Experiment 9 -  LM35 Temperature sensor</h3>

<h4 id="components-required-5">Components Required</h4>
<ul>
  <li>Arduino Uno Board</li>
  <li>LM35 Sensor</li>
  <li>Breadboard*1</li>
  <li>Breadboard Jumper Wire*3</li>
  <li>USB cable*1</li>
</ul>


<h4 id="code-8">Code</h4>
<pre><code class="language-ino">
int sensorPin = 0; // initialize analog pin 0 for LM35 temperature sensor
void setup()
{
Serial.begin(9600);// set baud rate at”9600”
}
void loop()
{
int val;// define variable
int dat;// define variable
val=analogRead(sensorPin);// read the analog value of the sensor and assign it to val
dat=(125*val)&gt;&gt;8;// temperature calculation formula
Serial.print("Tep");// output and display characters beginning with Tep
Serial.print(dat);// output and display value of dat
Serial.println("C");// display “C” characters
delay(500);// wait for 0.5 second
}

</code></pre>
<h3 id="experiment-10----ir-remote-control-using-tsop">Experiment 10 -  IR Remote Control Using TSOP</h3>

<h4 id="components-required-6">Components Required</h4>
<ul>
  <li>Arduino Uno Board</li>
  <li>TSOP Sensor</li>
  <li>LED*4</li>
  <li>resistor(220 ohm)*4</li>
  <li>Breadboard*1</li>
  <li>Breadboard Jumper Wire*8</li>
  <li>USB cable*1</li>
  <li>
    
  </li>
</ul>



<h4 id="code-9">Code</h4>
<pre><code class="language-ino">#include &lt;IRremote.h&gt;

const int RECV_PIN = 4 ;
int led1 = 5;
int led2 = 6;
int led3 = 7;
int led4 = 8;
int itsONled[] = {0,0,0,0,0};

#define code1  48511
#define code2  38079
#define code3  49371
#define code4  15355



IRrecv irrecv(RECV_PIN);
decode_results results;

void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  pinMode(led1,OUTPUT);
  pinMode(led2,OUTPUT);
  pinMode(led3,OUTPUT);
  pinMode(led4,OUTPUT);

  irrecv.enableIRIn();

}

void loop() {


  if (irrecv.decode(&amp;results)) {
        unsigned int value = results.value;
        switch(value) {
           case code1:
             if(itsONled[1] == 1) {        // if first led is on then
                digitalWrite(led1, LOW);   // turn it off when button is pressed
                itsONled[1] = 0;           // and set its state as off
             } else {                      // else if first led is off
                 digitalWrite(led1, HIGH); // turn it on when the button is pressed
                 itsONled[1] = 1;          // and set its state as on
             }
              break; 
           case code2:
             if(itsONled[2] == 1) {
                digitalWrite(led2, LOW);
                itsONled[2] = 0;
             } else {
                 digitalWrite(led2, HIGH);
                 itsONled[2] = 1;
             }
              break;
           case code3:
             if(itsONled[3] == 1) {
                digitalWrite(led3, LOW);
                itsONled[3] = 0;
             } else {
                 digitalWrite(led3, HIGH);
                 itsONled[3] = 1;
             }
              break;    
                case code4:
             if(itsONled[4] == 1) {
                digitalWrite(led4, LOW);
                itsONled[4] = 0;
             } else {
                 digitalWrite(led4, HIGH);
                 itsONled[4] = 1;
             }
              break;      
        }
        Serial.println(value); 
        irrecv.resume(); 
      }
    }

</code></pre>

<h3 id="experiment-11---potentiometer-analog-value-reading">Experiment 11 - Potentiometer analog Value Reading</h3>

<h4 id="components-required-7">Components Required</h4>
<ul>
  <li>Arduino Uno Board</li>
  <li>Potentiometer*1</li>
  <li>LED*1</li>
  <li>220Ω Resistor*1</li>
  <li>Breadboard*1</li>
  <li>Breadboard Jumper Wire*5</li>
  <li>USB cable*1</li>
</ul>

<h3 id="added-1">ADDED</h3>
<p>** i added a LED on output of potentiometer, so i can adjut LED’s brightness</p>


<h4 id="code-10">Code</h4>
<pre><code class="language-ino">
int vr = 0;
int val;
void setup() {
  // put your setup code here, to run once:
  pinMode(vr,INPUT);
  Serial.begin(9600);

}

void loop() {
  // put your main code here, to run repeatedly:
  val = analogRead(vr);
  Serial.println(val);

}
</code></pre>
<h3 id="experiment-12---7-segment-display">Experiment 12 - 7 Segment Display</h3>

<h4 id="components-required-8">Components Required</h4>
<ul>
  <li>Arduino Uno Board</li>
  <li>1-digit LED Segment Display*1</li>
  <li>LED*1</li>
  <li>220Ω Resistor*8</li>
  <li>Breadboard*1</li>
  <li>Breadboard Jumper Wire*10</li>
  <li>USB cable*1</li>
</ul>


<h4 id="code-11">Code</h4>
<pre><code class="language-ino">int a=10;// set digital pin 7 for segment a
int b=11;// set digital pin 6 for segment b
int c=5;// set digital pin 5 for segment c
int d=6;// set digital pin 10 for segment d
int e=7;// set digital pin 11 for segment e
int f=8;// set digital pin 8 for segment f
int g=9;// set digital pin 9 for segment g
int dp=4;// set digital pin 4 for segment dp

void digital_0(void) // display number 0
{
unsigned char j;
digitalWrite(a,HIGH);
digitalWrite(b,HIGH);
digitalWrite(c,HIGH);
digitalWrite(d,HIGH);
digitalWrite(f,HIGH);
digitalWrite(e,HIGH);
digitalWrite(g,LOW);
digitalWrite(dp,LOW);
}
void digital_1(void) // display number 1
{
unsigned char j;
digitalWrite(a,LOW);
digitalWrite(b,HIGH);
digitalWrite(c,HIGH);
digitalWrite(d,LOW);
digitalWrite(e,LOW);
digitalWrite(f,LOW);
digitalWrite(g,LOW);
digitalWrite(dp,LOW);
}
void digital_2(void) // display number 2
{
unsigned char j;
digitalWrite(b,HIGH);
digitalWrite(a,HIGH);
digitalWrite(c,LOW);
digitalWrite(d,HIGH);
digitalWrite(g,HIGH);
digitalWrite(dp,LOW);
digitalWrite(e,HIGH);
digitalWrite(f,LOW);
}
void digital_3(void) // display number 3
{digitalWrite(g,HIGH);
digitalWrite(a,HIGH);
digitalWrite(b,HIGH);
digitalWrite(c,HIGH);
digitalWrite(d,HIGH);
digitalWrite(dp,LOW);
digitalWrite(f,LOW);
digitalWrite(e,LOW);
}
void digital_4(void) // display number 4
{digitalWrite(c,HIGH);
digitalWrite(b,HIGH);
digitalWrite(f,HIGH);
digitalWrite(g,HIGH);
digitalWrite(dp,LOW);
digitalWrite(a,LOW);
digitalWrite(e,LOW);
digitalWrite(d,LOW);
}
void digital_5(void) // display number 5
{
unsigned char j;
digitalWrite(a,HIGH);
digitalWrite(b, LOW);
digitalWrite(c,HIGH);
digitalWrite(d,HIGH);
digitalWrite(e, LOW);
digitalWrite(f,HIGH);
digitalWrite(g,HIGH);
digitalWrite(dp,LOW);
}
void digital_6(void) // display number 6
{
unsigned char j;
for(j=7;j&lt;=11;j++)
digitalWrite(j,HIGH);
digitalWrite(c,HIGH);
digitalWrite(dp,LOW);
digitalWrite(b,LOW);
}
void digital_7(void) // display number 7
{
unsigned char j;
digitalWrite(c,HIGH);
digitalWrite(b,HIGH);
digitalWrite(f,LOW);
digitalWrite(g,LOW);
digitalWrite(dp,LOW);
digitalWrite(a,HIGH);
digitalWrite(e,LOW);
digitalWrite(d,LOW);

}
void digital_8(void) // display number 8
{
unsigned char j;
for(j=5;j&lt;=11;j++)
digitalWrite(j,HIGH);
digitalWrite(dp,LOW);
}
void digital_9(void) // display number 5
{
unsigned char j;
digitalWrite(a,HIGH);
digitalWrite(b,HIGH);
digitalWrite(c,HIGH);
digitalWrite(d,HIGH);
digitalWrite(e, LOW);
digitalWrite(f,HIGH);
digitalWrite(g,HIGH);
digitalWrite(dp,LOW);
}
void setup()
{
int i;// set variable
for(i=4;i&lt;=11;i++)
pinMode(i,OUTPUT);// set pin 4-11as “output”
}
void loop()
{
while(1)
{
digital_0();// display number 0
delay(1000);// wait for 1s
digital_1();// display number 1
delay(1000);// wait for 1s
digital_2();// display number 2
delay(1000); // wait for 1s
digital_3();// display number 3
delay(1000); // wait for 1s
digital_4();// display number 4
delay(1000); // wait for 1s
digital_5();// display number 5
delay(1000); // wait for 1s
digital_6();// display number 6
delay(1000); // wait for 1s
digital_7();// display number 7
delay(1000); // wait for 1s
digital_8();// display number 8
delay(1000); // wait for 1s
digital_9();// display number 9
delay(1000); // wait for 1s
}}

</code></pre>
<h3 id="assignment-1---automatic-night-lamp">Assignment 1 - Automatic Night Lamp</h3>

<h4 id="components-required-9">Components Required</h4>
<ul>
  <li>Arduino Uno Board</li>
  <li>Photo Resistor*1</li>
  <li>Red M5 LED*1</li>
  <li>10KΩ Resistor*1</li>
  <li>220Ω Resistor*1</li>
  <li>Breadboard*1</li>
  <li>Breadboard Jumper Wire*5</li>
  <li>USB cable*1</li>
</ul>

<p>LDR</p>



<h4 id="code-12">Code</h4>
<pre><code class="language-ino">int led = 4;
int ldr = 0;
int ldr_value;
void setup() {
  // put your setup code here, to run once:
  pinMode(led,OUTPUT);
  pinMode(ldr,INPUT);
  Serial.begin(9600);

}

void loop() {
  // put your main code here, to run repeatedly:
  ldr_value = analogRead(ldr);
  Serial.println(ldr_value);

  if(ldr_value &lt; 150){
    digitalWrite(led,HIGH);
    
  }else{
    digitalWrite(led,LOW);
  }

}

}
</code></pre>

<h3 id="assignment-2-digital-dice-using-7-segment-display">Assignment 2 Digital Dice Using 7 Segment Display</h3>

<h4 id="components-required-10">Components Required</h4>
<ul>
  <li>Arduino Uno Board</li>
  <li>7 Segment Display</li>
  <li>LED*1</li>
  <li>220Ω Resistor*8</li>
  <li>Breadboard*1</li>
  <li>Breadboard Jumper Wire*12</li>
  <li>USB cable*1</li>
</ul>


<h4 id="code-13">Code</h4>
<pre><code class="language-ino">int a=10;// set digital pin 7 for segment a
int b=11;// set digital pin 6 for segment b
int c=5;// set digital pin 5 for segment c
int d=6;// set digital pin 10 for segment d
int e=7;// set digital pin 11 for segment e
int f=8;// set digital pin 8 for segment f
int g=9;// set digital pin 9 for segment g
int dp=4;// set digital pin 4 for segment dp

int btnPin = 3;
int btnState;
long ran;

void digital_0(void) // display number 0
{
unsigned char j;
digitalWrite(a,HIGH);
digitalWrite(b,HIGH);
digitalWrite(c,HIGH);
digitalWrite(d,HIGH);
digitalWrite(f,HIGH);
digitalWrite(e,HIGH);
digitalWrite(g,LOW);
digitalWrite(dp,LOW);
}
void digital_1(void) // display number 1
{
unsigned char j;
digitalWrite(a,LOW);
digitalWrite(b,HIGH);
digitalWrite(c,HIGH);
digitalWrite(d,LOW);
digitalWrite(e,LOW);
digitalWrite(f,LOW);
digitalWrite(g,LOW);
digitalWrite(dp,LOW);
}
void digital_2(void) // display number 2
{
unsigned char j;
digitalWrite(b,HIGH);
digitalWrite(a,HIGH);
digitalWrite(c,LOW);
digitalWrite(d,HIGH);
digitalWrite(g,HIGH);
digitalWrite(dp,LOW);
digitalWrite(e,HIGH);
digitalWrite(f,LOW);
}
void digital_3(void) // display number 3
{digitalWrite(g,HIGH);
digitalWrite(a,HIGH);
digitalWrite(b,HIGH);
digitalWrite(c,HIGH);
digitalWrite(d,HIGH);
digitalWrite(dp,LOW);
digitalWrite(f,LOW);
digitalWrite(e,LOW);
}
void digital_4(void) // display number 4
{digitalWrite(c,HIGH);
digitalWrite(b,HIGH);
digitalWrite(f,HIGH);
digitalWrite(g,HIGH);
digitalWrite(dp,LOW);
digitalWrite(a,LOW);
digitalWrite(e,LOW);
digitalWrite(d,LOW);
}
void digital_5(void) // display number 5
{
unsigned char j;
digitalWrite(a,HIGH);
digitalWrite(b, LOW);
digitalWrite(c,HIGH);
digitalWrite(d,HIGH);
digitalWrite(e, LOW);
digitalWrite(f,HIGH);
digitalWrite(g,HIGH);
digitalWrite(dp,LOW);
}
void digital_6(void) // display number 6
{
unsigned char j;
for(j=6;j&lt;=11;j++)
digitalWrite(j,HIGH);
digitalWrite(c,HIGH);
digitalWrite(dp,LOW);
digitalWrite(b,LOW);
}

void setup()
{
int i;// set variable
for(i=4;i&lt;=11;i++)
pinMode(i,OUTPUT);// set pin 4-11as “output”
pinMode(3,INPUT);
randomSeed(analogRead(0));
Serial.begin(9600);
}
void loop()
{
  btnState = digitalRead(btnPin);
  if (btnState == HIGH){
    ran = random(1,7);
    Serial.println(ran);
    if (ran == 1){
      digital_1();
      delay(2000);
    }
    if (ran == 2){
      digital_2();
      delay(2000);
    }
    if (ran == 3){
      digital_3();
      delay(2000);
    }
    if (ran == 4){
      digital_4();
      delay(2000);
    }
    if (ran == 5){
      digital_5();
      delay(2000);
    }
    if (ran == 6){
      digital_6();
      delay(2000);
    }
  }
  else{
    digitalWrite(a,LOW);
    digitalWrite(b,LOW);
    digitalWrite(c,LOW);
    digitalWrite(d,LOW);
    digitalWrite(e,LOW);
    digitalWrite(f,LOW);
    digitalWrite(g,LOW);
    digitalWrite(dp,LOW);
    }
}





