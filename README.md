# GPP_Research

## Victory Calculation for skirmishes in Empire Earth

#### Introduction

The goal of this research was to create a program that would take 2 opposing groups of troops and calculate who would win in a fight.
This information could then be used to improve the game's AI. Helping it decide wether or not to commit to an engagement.
I chose to base this research in the game Empire Earth.

#### The Calculation

The technique i eventually settled on was a simplified battle simulation.
This would take the essential information 
"Troops per army, Hp of units, dmg of units, resistances, unit type" 
and use simple math to see which army would get fully killed first.

The calculation would take a unit from the army and use it to attack an opponent,
then it would do the same with a unit from the opposing army.
It repeats this process until there are no more units left in one or both armies.

#### The Results

The code predicted the correct outcome almost every time.
Innacuracies would mostly occur on situations where either the armies were very closely matched,
or the AI decided to run certain units around without attacking anything.
Here follow some examples:
