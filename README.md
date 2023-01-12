# GPP_Research

## Victory Calculation for skirmishes in Empire Earth

#### **Introduction**

The goal of this research was to create a program that would take 2 opposing groups of troops and calculate who would win in a fight.\
This information could then be used to improve the game's AI. Helping it decide wether or not to commit to an engagement.\
I chose to base this research in the game Empire Earth.

![image](https://user-images.githubusercontent.com/114000661/212171273-dcb7e6d1-2840-4eb7-a644-abe116947e55.png)

#### **The Calculation**

The technique i eventually settled on was a simplified battle simulation.\
This would take the essential information \
"Troops per army, Hp of units, dmg of units, resistances, unit type" \
and use simple math to see which army would get fully killed first.

The calculation would take a unit from the army and use it to attack an opponent,\
then it would do the same with a unit from the opposing army.\
It repeats this process until there are no more units left in one or both armies.

#### **The Results**

The code predicted the correct outcome almost every time.\
Innacuracies would mostly occur on situations where either the armies were very closely matched,\
or the AI decided to run certain units around without attacking anything.

Here follow some examples:\
**Army 0: 5 clubmen**\
**Army 1: 5 clubmen**

![image](https://user-images.githubusercontent.com/114000661/212170019-e17aa090-61b7-48e9-a7d2-c69f43f04fed.png)\
![image](https://user-images.githubusercontent.com/114000661/212169492-34f89f51-23aa-4c5c-87a1-eba6df960722.png)\
![image](https://user-images.githubusercontent.com/114000661/212169675-49a6c46d-0a78-4d4c-97a0-3afc21940524.png)


**Army 0: 4 clubmen , 2 rock_throwers**\
**Army 1: 5 spearmen**

![image](https://user-images.githubusercontent.com/114000661/212167319-95d7211a-51de-4403-8331-8253ff308b42.png)\
![image](https://user-images.githubusercontent.com/114000661/212170359-0ab8b362-319e-48db-8625-03807608be4f.png)\
![image](https://user-images.githubusercontent.com/114000661/212170458-a71152be-4612-4cf5-aba9-cb6114d21d47.png)


**Army 0: 5 clubmen**\
**Army 1: 5 spearmen**

![image](https://user-images.githubusercontent.com/114000661/212167319-95d7211a-51de-4403-8331-8253ff308b42.png)\
![image](https://user-images.githubusercontent.com/114000661/212170793-03f41e6c-b207-4a77-b4dc-5af80add0c92.png)\
![image](https://user-images.githubusercontent.com/114000661/212170852-595b8f9f-d6a7-443d-b587-0dc0d5795551.png)


**Army 0: 4 shortswords**\
**Army 1: 2 bronze_cavalry, 1 siple_archer**

![image](https://user-images.githubusercontent.com/114000661/212167319-95d7211a-51de-4403-8331-8253ff308b42.png)\
![image](https://user-images.githubusercontent.com/114000661/212171007-e9b54ef9-c9f5-4531-b635-3e0c5bd68a8f.png)\
![image](https://user-images.githubusercontent.com/114000661/212171096-44078851-6e5b-4905-aea7-e38365db78cf.png)



