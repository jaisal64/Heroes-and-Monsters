# CS611-<Assignment 3>
## <Monsters and Heroes>
---------------------------------------------------------------------------
<Jaisal Singh>
<jaisal@bu.edu>
<U60118211>

## Files
---------------------------------------------------------------------------
<A brief description of each file and what it does>

There is one main file and 6 files for classes that are explained below.
I have used my previous Tic Tac Toe code and only added the code for blackJack. I have added one new class: Playing cards.
Although I could have just used my previous gameBoard class, just for clarity I have created a new PlayingCards class. Rest all the csame classes are used.

Main:
It initializes the game by calling the gameEngine Class

Class1: gameBoard
generates the map with different types of cells and prints it


Class2: CHARACTER interface
Contains information about all the heroes and monsters

Class3: Hero class 
This abstract class implements character interface.


Class 3,4,5: Warrior, Paladin, Sorcerer
inherits the hero abstract class and creates the required hero classes

class 6 : monsters
abstract class that implements character interface

Class 7,8,9 : Dragon, Exoskeleton, Spirits
inherits the monsters class and creates the 3 types of monsters

Class10,11,12 : marketcell, commonCell, NoaccessCell
Creates 3 types of gamecells by inheriting from gamecell class

class 12: gamecell abstract class
initializes the gamecell class

Class 13: items abstract class
initializes class for all items in game

Class 14,15,16,17: armor, weapons, <<spells>>, potions
inherits items and creates classes for different items

class 18,19,20: fireSpell, IceSpell, Lightning Spell
inherits the spells class and creates different class for different spells

Class21: battle class
used for everything in the battle in game

class 22 market
has methods to implement the market rules 




## Notes
---------------------------------------------------------------------------
1. <Files to be parsed should be stored in ConfigFiles, for parser class to
read class>

1. Map is extendible between 3 and 10 size square grid.
2. number of heroes can be between 1 and 6.
3. I have not been able to do error catching for invalid inputs eveywhere.
4. Have not been able to implement unique markets due to lack of time.
5. Have used character interface that is inherited by abstract hero and monsters classes that are further inherited. Some abstract functions have also been used.

## How to compile and run
---------------------------------------------------------------------------
1. Navigate to the directory "src" after unzipping the files
2. Run the following instructions:
<Example below>
javac *.java
java Main

Java version Used to compile and run: JAVA 17 or java 8 im not fully sure.

## Input/Output Example
---------------------------------------------------------------------------
<Place here an example of how the program runs. Include both its
outputs and correctly formatted inputs. Please clearly mark the inputs.>


Welcome to Heroes and Monsters!
Enter size of NxN map between 3 and 10
Input:8

Welcome to Heroes and Monsters! How many heroes would you like to play with? Enter a number between 1 and 6
Input: 3

+---++---++---++---++---++---++---++---+
| P || M || C || M || C || I || C || M |
+---++---++---++---++---++---++---++---+
| C || M || C || M || C || M || C || I |
+---++---++---++---++---++---++---++---+
| C || M || C || M || C || M || C || M |
+---++---++---++---++---++---++---++---+
| C || I || C || M || C || M || C || M |
+---++---++---++---++---++---++---++---+
| C || M || C || I || C || M || C || M |
+---++---++---++---++---++---++---++---+
| C || M || C || M || C || I || C || M |
+---++---++---++---++---++---++---++---+
| C || M || C || M || C || M || C || I |
+---++---++---++---++---++---++---++---+
| C || M || C || M || C || M || C || M |

Controls: w/s/a/d for up/down/left/right. i: hero info, e: Apply Weapon/Armor/Potion , q: quit


