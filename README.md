

Overview

Game of Thrones is a hit fantasy tv show based on the equally famous book series "A Song of Fire and Ice" by George RR Martin. The show is well known for its vastly complicated political landscape, large number of characters, and its frequent character deaths.

Data Sources

This dataset combines three sources of data, all of which are based on information from the book series.

Firstly, there is battles.csv which contains Chris Albon's "The War of the Five Kings" Dataset, which can be found here: https://github.com/chrisalbon/war_of_the_five_kings_dataset . Its a great collection of all of the battles in the series.
Secondly we have character-deaths.csv from Erin Pierce and Ben Kahle. This dataset was created as a part of their Bayesian Survival Analysis which can be found here: http://allendowney.blogspot.com/2015/03/bayesian-survival-analysis-for-game-of.html
Finally we have a more comprehensive character dataset with character-predictions.csv. This comes from the team at A Song of Ice and Data who scraped it from http://awoiaf.westeros.org/ . It also includes their predictions on which character will die, the methodology of which can be found here: https://got.show/machine-learning-algorithm-predicts-death-game-of-thrones
What insights about the complicated political landscape of this fantasy world can you find in this data?

Of course, it goes without saying that this dataset contains spoilers ;)
Released Under CC0: Public Domain License



battles.csv
File size:
8.35 KB
Description:
This csv contains information about all of the battles in game of thrones:

name: String variable. The name of the battle.
year: Numeric variable. The year of the battle.
battle_number: Numeric variable. A unique ID number for the battle.
attacker_king: Categorical. The attacker's king. A slash indicators that the king charges over the course of the war. For example, "Joffrey/Tommen Baratheon" is coded as such because one king follows the other in the Iron Throne.
defender_king: Categorical variable. The defender's king.
attacker_1: String variable. Major house attacking.
attacker_2: String variable. Major house attacking.
attacker_3: String variable. Major house attacking.
attacker_4: String variable. Major house attacking.
defender_1: String variable. Major house defending.
defender_2: String variable. Major house defending.
defender_3: String variable. Major house defending.
defender_4: String variable. Major house defending.
attacker_outcome: Categorical variable. The outcome from the perspective of the attacker. Categories: win, loss, draw.
battle_type: Categorical variable. A classification of the battle's primary type. Categories: *pitched_battle*: Armies meet in a location and fight. This is also the baseline category. ambush: A battle where stealth or subterfuge was the primary means of attack. siege: A prolonged of a fortied position. razing: An attack against an undefended position
major_death: Binary variable. If there was a death of a major figure during the battle.
major_capture: Binary variable. If there was the capture of the major figure during the battle.
attacker_size: Numeric variable. The size of the attacker's force. No distinction is made between the types of soldiers such as cavalry and footmen.
defender_size: Numeric variable. The size of the defenders's force. No distinction is made between the types of soldiers such as cavalry and footmen.
attacker_commander: String variable. Major commanders of the attackers. Commander's names are included without honoric titles and commandders are seperated by commas.
defender_commander: String variable. Major commanders of the defener. Commander's names are included without honoric titles and commandders are seperated by commas.
summer: Binary variable. Was it summer?
location: String variable. The location of the battle.
region: Categorical variable. The region where the battle takes place. Categories: Beyond the Wall, The North, The Iron Islands, The Riverlands, The Vale of Arryn, The Westerlands, The Crownlands, The Reach, The Stormlands, Dorne
note: String variable. Coding notes regarding individual observations.




character-deaths.csv
File size:
37.96 KB
Description:
This csv contains information about characters and when they died.

Name: character name
Allegiances: character house
Death Year: year character died
Book of Death: book character died in
Death Chapter: chapter character died in
Book Intro Chapter: chapter character was introduced in
Gender: 1 is male, 0 is female
Nobility: 1 is nobel, 0 is a commoner
GoT: Appeared in first book
CoK: Appeared in second book
SoS: Appeared in third book
FfC: Appeared in fourth book
DwD: Appeared in fifth book



character-predictions.csv
File size:
210.49 KB
Description:
This csv takes an expanded view on character deaths, including predictions of how likely they are to die. (Prediction's come from A Song of Ice and Data's algorithm).

S.No
actual
pred
alive
plod
name
title
male
culture
dateOfBirth
DateoFdeath
mother
father
heir
house
spouse
book1
book2
book3
book4
book5
isAliveMother
isAliveFather
isAliveHeir
isAliveSpouse
isMarried
isNoble
age
numDeadRelations
boolDeadRelations
isPopular
popularity
isAlive


