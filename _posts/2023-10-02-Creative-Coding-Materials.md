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
- The other subjects will be added once they are covered.

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

