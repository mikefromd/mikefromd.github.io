---
layout: post
title: "Creative Coding Materials"
categories: WebDev 
---

This post here contains links to repositories that provide explanations and materials for the Creative Coding class.
Each subject is described in a separate repository.

### List of subjects:
- [Web: Front-End Design with HTML and CSS](https://mikefromd.github.io/Web_FrontEnd/)
- [TigerJython](https://github.com/mikefromd/TJ_Content/)
- [MAX](https://github.com/mikefromd/GPC5L05-main/tree/main)
- [MAX/MSP](https://github.com/mikefromd/MAX-MSP-Materials)
- [MAX BEAP modules](https://github.com/mikefromd/MAX-BEAP)
- [Vocoder and Visual Effects with MAX/MSP/BEAP](https://github.com/mikefromd/Vocoder)
- The other subjects will be added once they are covered.


### Various Materials for Scratch and Python on CodeClub

[This link](https://projects.raspberrypi.org/en/codeclub) brings you to the CodeClub website with a big choice of projects in Scratch, HTML/CSS, Python and other languages and environments.

The projects make often use of the p5 library to display and interact with graphics. Here is an example. the import statement and the two function definitions `def setup():` and `def draw():` as well as the call to `run()` at the end are mandatory elements of a skript using p5.

The p5 functions needed for the projects are all explained in detail step-by-step. 

```python
#!/bin/python3

from p5 import *
from random import randint

def setup():  
    size(640, 360)  
    no_stroke()  
    background(204)  

def draw():  
    fill(randint(0,255), randint(0,127), randint(0,51), 127)  
    circle_size = randint(10, 80)  
    ellipse(mouse_x, mouse_y, circle_size, circle_size)  

def mouse_pressed():
    background(204)
  
run()  
```

#### Here are the three projects I suggest you to choose from for today:

1. [Rocket launch](https://projects.raspberrypi.org/en/projects/rocket-launch) - Interactie simulation of a rocket launch, did you provide enough fuel?
2. [Make a face](https://projects.raspberrypi.org/en/projects/make-a-face) - Design your own interactive mask
3. [Don't collide (**)](https://projects.raspberrypi.org/en/projects/dont-collide/0) - Astro shooter type of game.

Projects one and two are good as an introduction, project three is rather challenging, but really interesting. There are a lot of explanations given on the website, so you can tackle all of them.



### Games:

#### RPG Games (Role Player Game)

A role-playing game (RPG) is a game in which players take the roles of characters in a fictional setting. Players are acting out these roles within a narrative, either through literal acting or through a process of structured decision-making regarding character development. Actions taken within many games succeed or fail according to a formal system of rules and guidelines.

Coming in a big variety, they started off with text-based games, nowadays many of them are visual games with varying storylines.

Today, we use the coding learning platform CodeClub that offers two classes that will lead you through the process of creating a RPG game. One offering is using Python to create a text-based "classic" RPG game, the other option is using Scratch. You can choose.

The Python version of the game will also run on TigerJython, so do not forget to copy and paste your final version of the game on your computer and save it in a file. TigerJython's text input is more powerful than the simple Python input, so you may tweak the code a  bit to make it look smoother.

##### Dictionary

A key language element to deal with this game is a *Dictionary*. While a [list](https://programmierkonzepte.ch/engl/index.php?inhalt_links=navigation.inc.php&inhalt_mitte=grafik/listen.inc.php) contains elements and you can access each list element by an index (whole number) `listElement = list[3]`, dictionaries consist out of key-value pairs `dict = {"key1":"value1", "key2":"value2", ...}`. The key can be anything, mostly a string and replaces the index to access the value. The example here gives you an idea on how this looks like. [here](https://programmierkonzepte.ch/engl/index.php?inhalt_links=navigation.inc.php&inhalt_mitte=internet/search.inc.php) you find a short introduction with some examples to give you the means to work on the Python game below.

```python
lexicon = {"blau":"blue", "rot":"red", "gruen":"green", "gelb":"yellow"}

print "All entries:"
for key in lexicon:
    print(key + " -> " + lexicon[key])
while True:
    farbe = input("color (deutsch)?")
    if farbe in lexicon:
        print(farbe + " -> " + lexicon[farbe])
    else:
        print(farbe + " -> " + "(not translatable)")
```

Here are the two links that bring you to the respective websites:

##### Python Game from Codeclub
[RPG Role Player Game with Python](https://projects.raspberrypi.org/en/projects/rpg/0)

##### RPG with Scratch on CodeClub
[Role Player Game with Scratch](https://projects.raspberrypi.org/en/projects/create-your-own-world)

