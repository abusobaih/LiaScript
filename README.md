<!--
author:   Abeer Abusobaih

email:    aabusobaih@gmail.com

version:  0.0.1

language: en

narrator:  US English Female

comment:  Try to write a short comment about
          your course, multiline is also okay.

link:     https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.css

script:   https://cdn.jsdelivr.net/chartist.js/latest/chartist.min.js

import:   https://raw.githubusercontent.com/liaTemplates/AVR8js/main/README.md

-->

# Arduino for Kids

The objective of the course is to make

Please see the [Docs](https://liascript.github.io/course/?https://raw.githubusercontent.com/liaScript/docs/master/README.md)
to find out what is possible in [LiaScript](https://liascript.github.io).

If you want to use instant help in your Atom IDE, please type **lia** to see all available shortcuts.

``` cpp
void setup() {
  Serial.begin(9600);
}

void loop() {
   while (Serial.available() > 0 ) {

     String str = Serial.readString();

     if (str.equals("send")) {
        Serial.println("identified");
     } else {
        Serial.println("unknown");
     }
   }
}
```
@AVR8js.sketch

``` cpp
void setup() {
  Serial.begin(9600);
}

void loop() {
   while (Serial.available() > 0 ) {

     String str = Serial.readString();

     if (str.equals("send")) {
        Serial.println("identified");
     } else {
        Serial.println("unknown");
     }
   }
}
```
@AVR8js.sketch


## Markdown

You can use common [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) syntax to create your course, such as:

1. Lists
2. ordered or

   * unordered
   * ones ...


| Header 1 | Header 2 | asdfasf | asdfafsd                            |
|:-------- | --------:| ------- | ----------------------------------- |
| Item 1   |   Item 2 | asdasdf |                                     |
|          |          |         |                                     |
|          |          |         |                                     |
|          |          |         |                                     |
|          |          |         | kjlbhlkjhlkjhlkh jlh lkjh lkh lhljh |
|          |          |         |                                     |
|          |          |         |                                     |


Images:

![images](https://farm2.static.flickr.com/1618/26701766821_7bea494826.jpg)

![image example](pic/image.jpg)


    {{|> Arabic Female}}
عبير ..... اول اختبار

_ Hello _

## Styling

<!-- class = "animated rollIn" style = "animation-delay: 2s; color: purple" -->
The whole text-block should appear in purple color and with a wobbling effect.
Which is a **bad** example, please use it with caution ...
~~ only this is red ;-) ~~ <!-- class = "animated infinite bounce" style = "color: red;" -->

## Charts

Use ASCII-Art to draw diagrams:

                                    Multiline
    1.9 |    DOTS
        |                 ***
      y |               *     *
      - | r r r r r r r*r r r r*r r r r r r r
      a |             *         *
      x |            *           *
      i | B B B B B * B B B B B B * B B B B B
      s |         *                 *
        | *  * *                       * *  *
     -1 +------------------------------------
        0              x-axis               1

## Quizzes

### A Textquiz

What did the **fish** say when he hit a **concrete wall**?

    [[dam]]

### Multiple Choice

Just add as many points as you wish:

    [[X]] Only the **X** marks the correct point.
    [[ ]] Empty ones are wrong.
    [[X]] ...

### Single Choice

Just add as many points as you wish:

    [( )] ...
    [(X)] <-- Only the **X** is allowed.
    [( )] ...

## Executable Code

### Extensions

     --{{0}}--
But you can also include other features such as spoken text.

      --{{1}}--
Insert any kind of audio file:

       {{1}}
?[audio](https://bigsoundbank.com/UPLOAD/mp3/1068.mp3)


     --{{2}}--
Even videos or change the language completely.

       {{2-3}}
!?[video](https://www.youtube.com/watch?v=bICfKRyKTwE)

??[asdfasf](https://sketchfab.com/3d-models/al-khazneh-the-treasury-petra-39ef0f6c82224860ad49039d2534046d)


      --{{3 Russian Female}}--
Первоначально создан в 2004 году Джоном Грубером (англ. John Gruber) и Аароном
Шварцем. Многие идеи языка были позаимствованы из существующих соглашений по
разметке текста в электронных письмах...


    {{3}}
Type "voice" to see a list of all available languages.

## External links

A drawing example, for demonstrating that any JavaScript library can be used, also for drawing.

```javascript
// Initialize a Line chart in the container with the ID chart1
new Chartist.Line('#chart1', {
  labels: [1, 2, 3, 4],
  series: [[100, 120, 180, 200]]
});

// Initialize a Line chart in the container with the ID chart2
new Chartist.Bar('#chart2', {
  labels: [1, 2, 3, 4],
  series: [[5, 2, 8, 3]]
});
```
<script>@input</script>

<div class="ct-chart ct-golden-section" id="chart1"></div>
<div class="ct-chart ct-golden-section" id="chart2"></div>


### Projects

You can make your code executable and define projects:

``` js     -EvalScript.js
let who = data.first_name + " " + data.last_name;

if(data.online) {
  who + " is online"; }
else {
  who + " is NOT online"; }
```
``` json    +Data.json
{
  "first_name" :  "Sammy",
  "last_name"  :  "Shark",
  "online"     :  true
}
```
<script>
  // insert the JSON dataset into the local variable data
  let data = @input(1);

  // eval the script that uses this dataset
  eval(`@input(0)`);
</script>

## More

Find out what you can even do more with quizzes:

https://liascript.github.io/course/?https://raw.githubusercontent.com/liaScript/docs/master/README.md
