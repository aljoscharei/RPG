[[Programmieren MOC]]
[[Python MOC]]
[[Symbaroum Monsters MOC]]
[[202109281009 Aktuelle Projekte]]

[[Symbaroum Monster Fey Beast]]
[[lich lair actions]]
[[Symbaroum Monster Dragon]]
[[Symbaroum Monster Barbarian Village guard]]
[[Symbaroum Monster Village Witch]]
[[Symbaroum Monster Aboar]]

the core document [[vipinajayakumar-com-Parsing text with Python.pdf]]  Vipin Ajayakumar https://www.vipinajayakumar.com/parsing-text-with-python/
	lookaheads [[regular-expressions-info-Lookahead and Lookbehind Zero-Length Assertions.pdf]]
parsers [[tomassetti-me-Parsing In Python Tools And Libraries.pdf]]
string slicing [[digitalocean-com-How To Index and Slice Strings in Python 3.pdf]]
[[remove item from list.pdf]]
[[list comprehensions.pdf]]


Statblock mit regex finden
opening the file:

```python
with open('sample.txt') as file:
    file_contents = file.read()
    print(file_contents)
```

```
Sample text

A selection of students from Riverdale High and Hogwarts took part in a quiz. 
Below is a record of their scores.

School = Riverdale High
Grade = 1
Student number, Name
0, Phoebe
1, Rachel

Student number, Score
0, 3
1, 7

Grade = 2
Student number, Name
0, Angela
1, Tristan
2, Aurora

Student number, Score
0, 6
1, 3
2, 9

School = Hogwarts
Grade = 1
Student number, Name
0, Ginny
1, Luna

Student number, Score
0, 8
1, 7

Grade = 2
Student number, Name
0, Harry
1, Hermione

Student number, Score
0, 5
1, 10

Grade = 3
Student number, Name
0, Fred
1, George

Student number, Score
0, 0
1, 0
```


```python
# set up regular expressions
# use https://regexper.com to visualise these if required
rx_dict = {
    'school': re.compile(r'School = (?P<school>.*)\n'),
    'grade': re.compile(r'Grade = (?P<grade>\d+)\n'),
    'name_score': re.compile(r'(?P<name_score>Name|Score)'),
}
```

```python
def _parse_line(line):
    """
    Do a regex search against all defined regexes and
    return the key and match result of the first matching regex

    """

    for key, rx in rx_dict.items():
        match = rx.search(line)
        if match:
            return key, match
    # if there are no matches
    return None, None
```


```python


def parse_file(filepath):
    """
    Parse text at given filepath

    Parameters
    ----------
    filepath : str
        Filepath for file_object to be parsed

    Returns
    -------
    data : pd.DataFrame
        Parsed data

    """

    data = []  # create an empty list to collect the data
    # open the file and read through it line by line
    with open(filepath, 'r') as file_object:
        line = file_object.readline()
        while line:
            # at each line check for a match with a regex
            key, match = _parse_line(line)

            # extract school name
            if key == 'school':
                school = match.group('school')

            # extract grade
            if key == 'grade':
                grade = match.group('grade')
                grade = int(grade)

            # identify a table header 
            if key == 'name_score':
                # extract type of table, i.e., Name or Score
                value_type = match.group('name_score')
                line = file_object.readline()
                # read each line of the table until a blank line
                while line.strip():
                    # extract number and value
                    number, value = line.strip().split(',')
                    value = value.strip()
                    # create a dictionary containing this row of data
                    row = {
                        'School': school,
                        'Grade': grade,
                        'Student number': number,
                        value_type: value
                    }
                    # append the dictionary to the data list
                    data.append(row)
                    line = file_object.readline()

            line = file_object.readline()

        # create a pandas DataFrame from the list of dicts
        data = pd.DataFrame(data)
        # set the School, Grade, and Student number as the index
        data.set_index(['School', 'Grade', 'Student number'], inplace=True)
        # consolidate df to remove nans
        data = data.groupby(level=data.index.names).first()
        # upgrade Score from float to integer
        data = data.apply(pd.to_numeric, errors='ignore')
    return data
```


have infile, finder containing outfile and vscode open
![[Bildschirmfoto 2022-09-16 um 09.23.21.png]]

```python
# create a conda environment in Shell:

# $ brew install miniconda.

# $ conda conda create -n myenv python=3.9 pandas (oder 3.10 oder whatever).

# in the end was not necessary

# delete environment with

# $ conda env remove -n myenv

# choose interpreter by clicking in right bottom corner in vscode

  

# it is more elegant to store the searches in a dict. like so

# https://www.vipinajayakumar.com/parsing-text-with-python/

  

# rx_dict = {

# 'school': re.compile(r'School = (?P<school>.*)\n'),

# 'grade': re.compile(r'Grade = (?P<grade>\d+)\n'),

# 'name_score': re.compile(r'(?P<name_score>Name|Score)'),

# }

  

# Regex: ```statblock(.|\n)*```

  

# but in the end i was running the search only once, so re.compile was

# not faster

# the regexes were build with https://regex101.com/

# it is better not to fiddle to find the perfect regex

# a major problem ist that the only way to include sth in the search

# patter that is not supposed to be in the result is lookaheads and

# lookbehinds like (?=SEARCH_PATTERN), or (?<=SEARCH_PATTERN). Those

# must be known length. OR operators are ok but not .* or such quantifiers

# see: https://www.regular-expressions.info/lookaround.html

# It is better and more readable to get a chunk and then get rid of the

# undesirable stuff with string

# methods.

# All of this is a hot mess. It is really not DRY. I mosty copied pasted working code

# and modifierd when it didn't work.

  
  

# What to do to make it work.

# Copy the text to be parsed in the infile.txt The statblock is written to the outfile.

  

# ToDo Filename for name:

# ToDo Spells

# ToDo bonus_actions:

# To tidy up it might make sense to re-read in the statblock line by line.

  
  

# from curses.ascii import isspace

# from distutils.dir_util import copy_tree

# import pandas as pd

import re

  

# outfile.txt infile.txt

from fileinput import filename

  

BASEPATH = r"/Users/aljoschabeyer/Library/Mobile Documents/iCloud~md~obsidian/Documents/Zettel/Symbaroum Monsters/"

  

with open(BASEPATH + "infile.txt") as file:

file_contents = file.read()

# print(file_contents)

  
  

Size_Type = re.search(

r"(tiny|small|medium|large|huge|gargantuan) (Phenomenon|Aberration|Abomination|Beast|Celestial|Construct|Dragon|Elemental|Fey|Fiend|Giant|Humanoid|Human|Goblin|Ogre|Troll|Monstrosity|Ooze|Plant|Undead)",

file_contents,

re.I,

)

ac = re.search(r"Armor Class(\*\*)? (\d+)", file_contents, flags=re.I)

Hp = re.search(r"Hit Points( |\*+)+\d+.*\)", file_contents, re.I)

Speed = re.search(r"\n\s?(\*\*)?Speed(\*\*)?.*\n", file_contents, re.I)

Stats = re.search(r"\|.*\d+.*\n", file_contents, re.M)

Saves = re.search(r"(?<=Saving Throws)(.|\n)*(?=Skills)", file_contents, re.I)

Skills = re.search(r"(?<=Skills).*(\n|Languages)", file_contents, re.I)

DVs = re.search(r"(?<=Damage Vulnerabilities).*(\n)", file_contents, re.I)

DRs = re.search(r"(?<=Damage Resistances).*(\n)", file_contents, re.I)

DIs = re.search(r"(?<=Damage Immunities).*(\n)", file_contents, re.I)

CIs = re.search(r"(?<=Condition Immunities).*(\n)", file_contents, re.I)

Senses = re.search(r"(?<=Senses).*?(Languages|\n)", file_contents, re.I)

Langs = re.search(r"(?<=Languages).*\n", file_contents, re.I)

Equipment = re.search(r"(?<=Equipment).*\n", file_contents, re.I)

Cr = re.search(r"(?<=Challenge)( |\*+)*?\d+", file_contents, re.I)

Traits = re.search(

r"((?<=Equipment)|(?<=Challenge))((.|\n)*?)(?=actions)", file_contents, re.I

)

Spells = re.search(

r"(?<=spells)|(?<=spellcasting)((.|\n)*?)((?=actions)|(?=action))",

file_contents,

re.I,

)

actions = re.search(

r"(?<=actions)(.|\n)*?((?=reactions)|(?=legendary)|(?=bonus)|$)", file_contents, re.I

)

Legendary = re.search(

r"(?<=Legendary actions)(.|\n)*((?=reactions)|(?=bonus)|$)", file_contents, re.I

)

Reactions = re.search(

r"(?<=reactions)(.|\n)*?((?=legendary)|(?=bonus)|$)", file_contents, re.I

)

# Bonus = re.search(r'(?<=Senses).*\n',file_contents,re.I)

# the resulting variables are match objects.

# https://docs.python.org/3/library/re.html#match-objects

# they are usable as boolean which I do at the top with the if..

# if the object is none because there was no match, then nothing gets

# added to the string s

# to see the match as string do: MATCH-OBJECT.group(0)

  

# now start building the output line by line. output is the string s

s = "```statblock\n"

s += "image: [[Wikilink To Image]]\n"

s += "name: \n"

if Size_Type:

SizeTypeString = Size_Type.group(0)

Size = re.search(r"(tiny|small|medium|large|huge|gargantuan)", SizeTypeString, re.I)

Type = re.search(

r"(Phenomenon|Aberration|Abomination|Beast|Celestial|Construct|Dragon|Elemental|Fey|Fiend|Giant|Humanoid|Human|Goblin|Ogre|Troll|Monstrosity|Ooze|Plant|Undead)",

SizeTypeString,

re.I,

)

if Size:

SizeString = Size.group(0)

s += "size: " + SizeString.strip() + "\n"

if Type:

TypeString = Type.group(0)

s += "type: " + TypeString.strip() + "\n"

s += "alignment:\n"

if ac:

ac = re.search(r"\d+", ac.group(0))

s += "ac: " + ac.group(0) + "\n"

if Hp:

HpString = Hp.group(0)

HitPoints = re.search(r"\s\d{1,3}", HpString, re.I)

s += "hp: " + HitPoints.group(0) + "\n"

HitDice = re.search(r"\(.*\)", HpString)

HitDiceString = HitDice.group(0)

s += "hit_dice: " + HitDiceString + "\n"

if Speed:

Speed = Speed.group(0)

Speed = Speed.replace("Speed", "")

Speed = Speed.replace("*", "")

Speed = Speed.strip()

s += "speed: " + Speed + "\n"

if Stats:

# Stats is very messy but I know that the odd numbers

# are the stats and the even numbers are the modifiers

# https://www.digitalocean.com/community/tutorials/how-to-index-and-slice-strings-in-python-3

# [start:end:stride]

# then formatting https://docs.python.org/3/library/string.html#format-string-syntax

StatsList = re.findall(r"\d+", Stats.group(0))

del StatsList[1::2]

StatString = "[{0},{1},{2},{3},{4},{5}]"

FormStatString = StatString.format(*StatsList) # the * ist important

s += "stats: " + FormStatString + "\n"

if Saves:

Saves = Saves.group(0)

Saves = Saves.replace("*", "")

Saves = Saves.strip()

Saves = Saves.replace(".", ",")

Saves = Saves.replace(";", ",")

Saves = Saves.split(",")

Saves = list(filter(None, Saves))

s += "saves:\n"

for save in Saves:

save = save.replace("+", ": ")

s += " - " + save + "\n"

if Skills:

Skills = Skills.group(0)

Skills = Skills.replace("*", "")

Skills = Skills.strip()

Skills = Skills.replace(".", ",")

Skills = Skills.replace(";", ",")

Skills = Skills.split(",")

Skills = list(filter(None, Skills))

s += "skillsaves:\n"

for skill in Skills:

skill = skill.replace("+", ": ")

s += " - " + skill + "\n"

if DVs:

DVs = DVs.group(0)

DVs = DVs.replace("Damage Vulnerabilites", "")

DVs = DVs.replace("*", "")

DVs = DVs.replace(":", "")

DVs = DVs.strip()

s += "damage_vulnerabilities: " + DVs + "\n"

if DRs:

DRs = DRs.group(0)

DRs = DRs.replace("Damage Resistances", "")

DRs = DRs.replace("*", "")

DRs = DRs.replace(":", "")

DRs = DRs.strip()

s += "damage_resistances: " + DRs + "\n"

if DIs:

DIs = DIs.group(0)

DIs = DIs.replace("Damage Immunities", "")

DIs = DIs.replace("*", "")

DIs = DIs.replace(":", "")

DIs = DIs.strip()

s += "damage_immunities: " + DIs + "\n"

if CIs:

CIs = CIs.group(0)

CIs = CIs.replace("Condition Immunities", "")

CIs = CIs.replace("*", "")

CIs = CIs.replace(":", "")

CIs = CIs.strip()

s += "condition_immunities: " + CIs + "\n"

if Senses:

Senses = Senses.group(0)

Senses = Senses.replace("Senses", "")

Senses = Senses.replace("Languages", "")

Senses = Senses.replace("*", "")

Senses = Senses.replace(":", "")

Senses = Senses.strip()

s += "senses: " + Senses + "\n"

if Langs:

Langs = Langs.group(0)

Langs = Langs.replace("Languages", "")

Langs = Langs.replace("*", "")

Langs = Langs.replace(":", "")

Langs = Langs.strip()

s += "languages: " + Langs + "\n"

if Equipment:

Equipment = Equipment.group(0)

Equipment = Equipment.replace("Equipment", "")

Equipment = Equipment.replace("*", "")

Equipment = Equipment.replace(":", "")

Equipment = Equipment.strip()

s += "equipment: " + Equipment + "\n"

if Cr:

Cr = Cr.group(0)

Cr = Cr.replace("Challenge", "")

Cr = Cr.replace("*", "")

Cr = Cr.strip()

s += "cr: " + Cr + "\n"

  

# for loop to add variable number of traits, actions etc.

# if found it easieast to split the block of text and then

# throw out list elements that were empty, or contained a keyword

# of another line.

# actually there are methods for deleting elements in lists

# https://note.nkmk.me/en/python-list-clear-pop-remove-del/

# https://note.nkmk.me/en/python-list-comprehension/

# but i had already started by building a loop that ignores

# undesirable elements with if...elif and continue

if Traits:

TraitsString = Traits.group(0).replace("#", "")

TraitsString = TraitsString.replace("*", "")

TraitsList = TraitsString.split("\n")

s += "traits:\n"

for item in TraitsList:

if not item:

continue

elif item.isspace():

continue

elif "XP" in item:

continue

elif "Manner" in item:

continue

elif "Shadow" in item:

continue

elif "Equipment" in item:

continue

elif "Challenge" in item:

continue

else:

item = item.strip()

TraitsName = re.search(r"[^\.]*", item)

TraitsNameString = TraitsName.group(0)

TraitsNameString = TraitsNameString.strip()

  

searchstring = r"(?<=" + re.escape(TraitsNameString) + r")(.|\n)*$"

TraitsDesc = re.search(searchstring, item, re.I)

# re.sub is so cool. In the doc it say that the replacement

# needs to be a function but empty string works.

# the returs a string to for once no need for .group(0)

TraitsDescString = re.sub(

r"^\. ", "", TraitsDesc.group(0), re.I

) # remove leading dots

TraitsDescString = TraitsDescString.strip()

s += " - name: " + TraitsNameString + "\n"

s += ' desc: "' + TraitsDescString + '"\n'

  

if actions:

actionsString = actions.group(0).replace("#", "")

actionsString = actionsString.replace("*", "")

actionsList = actionsString.split("\n")

s += "actions:\n"

for item in actionsList:

if not item or item.isspace():

continue

else:

item = item.strip()

actionName = re.search(r"[^\.]*", item)

actionNameString = actionName.group(0)

actionNameString = actionNameString.strip()

# actionNameString = actionNameString.replace('.','')

# actionNameString = actionNameString.strip()

  

searchstring = r"(?<=" + re.escape(actionNameString) + r")(.|\n)*$"

actionsDesc = re.search(searchstring, item, re.I)

actionsDescString = re.sub(

r"^\. ", "", actionsDesc.group(0), re.I

) # remove leading dots

# actionDescString = actionsDesc.group(0)

  

actionsDescString = actionsDescString.strip()

# actionDescString = actionDescString.replace('.','')

# actionDescString = actionDescString.strip()

# actionTupel.append(tuple([actionNameString,actionDescString]))

s += " - name: " + actionNameString + "\n"

s += ' desc: "' + actionsDescString + '"\n'

  

if Legendary:

LegendaryString = Legendary.group(0).replace("#", "")

LegendaryString = LegendaryString.replace("*", "")

LegendaryList = LegendaryString.split("\n")

s += "legendary_actions:\n"

for item in LegendaryList:

if not item or item.isspace():

continue

else:

item = item.strip()

LegendaryName = re.search(r"[^\.]*", item)

LegendaryNameString = LegendaryName.group(0)

LegendaryNameString = LegendaryNameString.strip()

  

searchstring = r"(?<=" + re.escape(LegendaryNameString) + r")(.|\n)*$"

LegendaryDesc = re.search(searchstring, item, re.I)

LegendaryDescString = re.sub(

r"^\. ", "", LegendaryDesc.group(0), re.I

) # remove leading dots

LegendaryDescString = LegendaryDescString.strip()

s += " - name: " + LegendaryNameString + "\n"

s += ' desc: "' + LegendaryDescString + '"\n'

  

if Reactions:

ReactionsString = Reactions.group(0).replace("#", "")

ReactionsString = ReactionsString.replace("*", "")

ReactionsString = ReactionsString.strip()

ReactionsList = ReactionsString.split("\n")

s += "reactions:\n"

for item in ReactionsList:

if not item or item.isspace():

continue

else:

item = item.strip()

ReactionsName = re.search(r"[^\.]*", item)

ReactionsNameString = ReactionsName.group(0)

ReactionsNameString = ReactionsNameString.strip()

  

searchstring = r"(?<=" + re.escape(ReactionsNameString) + r")(.|\n)*$"

ReactionsDesc = re.search(searchstring, item, re.I)

ReactionsDescString = re.sub(

r"^\. ", "", ReactionsDesc.group(0), re.I

) # remove leading dots

  

ReactionsDescString = ReactionsDescString.strip()

s += " - name: " + ReactionsNameString + "\n"

s += ' desc: "' + ReactionsDescString + '"\n'

s += "```"

  
  

writefile = open(BASEPATH + "outfile.md", "w")

writefile.write(s)

writefile.close()
```


