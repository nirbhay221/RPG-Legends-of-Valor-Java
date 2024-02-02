## Legends of Valor
---------------------------------------------------------------------------
## Files
---------------------------------------------------------------------------
1. Armor  - Armor class contains market armor arraylist and attributes necessary for creating the armor class . It contains Initialize armor inventory method , choose armor and market armor methods to populate the inventory of the heroes and market .
2. Board - Board class contains the methods to move the user accross different tiles and label the tiles as Market - where market method is invoked and you are directly taken to the market for shopping accessories (M), No Man's Land(N) - The place that is inaccessible to any Hero moving on the board   , Land - (L) - Land is the place where the dice is used to make that land a resting place to restore health , or a market to buy accessories , or a place for conflict between heroes and monsters.  
In this one the board class contains the  following tiles - Koulou (K), Cave(C) , Borders (X) , Bush (B) , Market (M) , Nexus (N) for heroes and villains , (H) - Hero for lane one , (W) - Hero for Lane two , (G) - Hero for lane three. 
(V) - Villain for lane one , (E) - Villain for lane two , (S) - Villain for lane three . Nexus has the market too . Also , in the game , when the hero gets on a  Koulou (K), Cave(C) or a Bush (B) tile , it will experience a certain level of increase in the some of the abilities .
Also in the User move , the user or the hero can now teleport to another lane to the hero  - This can happen randomly or with options , You can spawn back to nexus , Also you can spawn to the last teleport positions . Fainted heroes will respawn at the nexus and if some individual villain dies in the game , it will disappeaar from the board .
3. Characters - Character class is an abstract class that helps in creating the subclasses Heroes and Villains.In the villain move , you can change the movement to move down by changing the rndChoice in the board class in villain move so that there are no stack overflow errors .
4. CharacterStory- This class is used for creating a randomly generated story at each hero level when the level ends , it wil display an intro and outro for the random plot that continues in the game to make it exciting . 
5. DragonsDatabase - This is a monster's subclass that is used to create different typess of objects of the dragons .
6. ExoSkeletonDatabase - This is a ExoSkeleton's subclass that is used to create different typess of objects of the Exoskeletonss .
7. FireSpells -Fire spells class which is a subclass of spells contains market Fire spell arraylist and attributes necessary for creating the Fire spell class . It contains Initialize fire spell inventory method , choose fire spell and market fire spell methods to populate the inventory of the heroes and market .
8. Heroes -**You can make the hero weak as possible by playing with the ratios **Heroes is a subclass of Characters , it has all the features of the different types of Heroes and contains methods to attack the villain using different techniques  - Using weapons , hands , spells , and protection and defense is carried out with armor . These methods have a randomized value to increase the probability of risk in the game . You can choose different type of trait - Aggressive or Defensive , Also you can choose the type of hero you want to select using this class .
9. IceSpells - Ice spells class which is a subclass of spells contains market ice spell arraylist and attributes necessary for creating the ice class . It contains Initialize ice spell inventory method , choose ice spell and market Ice spell methods to populate the inventory of the heroes and market .
10. ItemInventory - Item Inventory class is used to contain all the items in the inventory . 
11. LightningSpells -Lightning spells class which is a subclass of spells contains market lightning spell arraylist and attributes necessary for creating the lightning spell class . It contains Initialize lightning spell inventory method , choose armor and market lightning spell methods to populate the inventory of the heroes and market .
12. Logic - It is the main class that handles all the events of heroes and villains . How they interact , and how all the users are updated each round , and how they can update their inventory and buy products from the market and update their money , other than that, it can be used to make the villains more powerful with increasing levels and also helps in making the heroes expendable to fight them and can have greater amount of weapons to fight the darkness.
13. Main - It is just use to invoke the start game method of the logic class .
It also involves the battle and increasing the level of heroes and monsters and logic class and board class are used to make the game move smoothly . Logic class helps in initiating the battle and moving on the board which will result in some events that you can observe on the board .
14. Market- it contains the array list to hold the weapons , spells , armors in order to populate the market class.
15. Paladins-It is a  subclass of the Heroes class which can be used to create different versions of the Paladins.
16. Potions - Potions class is used to initialize different potion objects, and contain methods to help the user choose different potions and help the market to be populated with potions each level .
17. Sorcerer - It is a  subclass of the Heroes class which can be used to create different versions of the sorcerers.
18. Spells - Spell class can be used to create a variation in the version of the spell object you want to create .
19. SpiritsDatabase - It is a  subclass of the Villains class which can be used to create different versions of the Spirits.
20. Villains-Potions class is used to initialize different potion objects, and contain methods to help the user choose different potions and help the market to be populated with potions each level .
21. Warrior - It is a  subclass of the Heroes class which can be used to create different versions of the warriors.
22. Weapons - Potions class is used to initialize different potion objects, and contain methods to help the user choose different potions and help the market to be populated with potions each level .
23. Sound Player : For adding sound to the game and foot steps.
24.CastSpellable : Interface for spells .
25.Choose Item : Interface for choosing an object .
26.Fightable : Interface used by heroes and villains.
27.ItemInitializable : Interface used for initializing the objects .
28.Marketable : Interface used by potions . 
29. Main Logic : Main Abstract game class.
## Notes
---------------------------------------------------------------------------
1. Most of the classes can be found in the PA4 folder .
2. I have implemented almost all the instructions mentioned in the pdf. But my formulas for spell attack , attack , defend can be a little different . Other than that at the start you can make the player choose one accessory from each of the inventory because they have that much money to buy for the initial selection . 
3.I have added the board which has Heroes as (H) that can move everywhere on the board in the specific lane ,it can move on the market (M) to buy weapons , armors , spells , potions .You cannot go to X which is the border you can only enter another lane with the help of the teleportation.
Excluding this I have added a little different formulas to make the villains powerful each round . Also none of the monsters can escape . I have added a feature for the heroes to escape which can be a possibility .
Also there is sound included in the game and the game includes two modes of teleportation , one at random and one with options . 
4. Each Hero has a specific characteristics that it chooses at each level . Also the game has three modes of difficulty to choose how powerful villains you want to play with .
You cannot move ahead unless you have killed all the monsters . each hero can kill one or more monsters . And if all of them faint , the game ends or if all of the villains die , all the heros can move ahead with the game with upgraded attributes . 
The starting menu allows the user to use it's inventory to equip or dequip weapons , armors , potions , spells as mentioned . 
Also I have created outro and intro for each level , And with increasing level above 5 , you can have randomized outro and intro based on different places mentioned in the code .
Also the market is populated each level with new and different weapons which will have enhanced characteristics . 
5.The XP here is used as level points which can be used to help in the attack for both monsters and heroes . 
6. Also if you get stuck anywhere you can use some number to move ahead since there are no infinite loops in the code so after a few small trials you can go ahead with the game depending upon the number of players taken into account.
7. Also spells and attacks are mended in such a way that some of the spells and attacks produced from hero side can be seen as an advantage to the monster depending upon the type of monsters. 
8. Holding weapons in hand is also added .
9 If you get stuck anywhere press "1" to move ahead in the game .
10 . Villain info is also printed.
11. You can change the double values in the villain and heroes attack method to see the difference in attacking .
12. There might be some gibberish , that was just for checking the testing inputs and outputs .
# How to compile and run
---------------------------------------------------------------------------
1. Navigate to the directory "pa4" after unzipping the files
2. Run the following instructions:
javac Main.java
java Main

## Input/Output Example
---------------------------------------------------------------------------
Case I : Teleportation :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
GAME : STARTS
It Enters
Sound should start!
Enter your Name : Please !
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Name : 1 Is that Correct ? 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Yes .
(2) No ,Please Change My Name.
-->
1
Choose the Difficulty Mode :
(1) Easy
(2) Normal
(3) Hard
-->

1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Introduction 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You are one of the hero (elite) . In order to protect the your homeland , it's your duty to fight the evil
Every Single one of your friends needs to be saved so that the town can live happily , a slight mistake can cause it to perish
All you need to do is get more experience and try to survive till the end and pass it on to the new generation .
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Type for your player :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1)Warrior
(2)Sorcerer
(3)Paladin
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Warrior!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Type for your player :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1)Gaerdal_Ironhand
(2)Sehanine_Monnbow
(3)Muamman_Duathall
(4)Flandal_Steelskin
(5)Undefeated_Yoj
(6)Eunoia_Cyn
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Gaerdal_Ironhand!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Trait for your player :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1)Strength
(2)Heavy Bones
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Strength!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Weapon for your player (At the start you can choose only one weapon):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Sword
(2) Bow
(3) Scythe
(4) Axe
(5) TSwords
(6) Dagger
->

1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Sword!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Enter 1 to continue:
1
Equip Some Weapon
Sword
Hands Occupied In :0
Ouput I1
Hands Occupied Output : 1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Armor for your player (At the start you can choose only one armor):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Platinum_Shield
(2) Breastplate
(3) Full_Body_Armor
(4) Wizard_Shield
(5) Guardian_Angel
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Platinum_Shield!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Enter 1 to continue:

1
Armors : In Inventory
Platinum_Shield
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Lightning Spell for your player (At the start you can choose only one Lightning Spell):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Lightning_Dagger
(2) Thunder_Blast
(3) Electric_Arrows
(4) Spark_Needles
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Lightning_Dagger!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
spell : LightningSpells@27d6c5e0
Enter 1 to continue:
1
LightningSpells : In Inventory
Lightning_Dagger
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Fire Spell for your player (At the start you can choose only one Fire Spell):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Flame_Tornado
(2) Breath_of_Fire
(3) Heat_Wave
(4) Lava_Comet
(5) Hell_Storm
->

1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Flame_Tornado!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Enter 1 to continue:
1
FireSpells : In Inventory
Flame_Tornado
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Ice Spell for your player (At the start you can choose only one Ice Spell):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Snow_Cannon
(2) Ice_Blade
(3) Frost_Blizzard
(4) Arctic_Storm
->

1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Snow_Cannon!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
-->
1
IceSpells : In Inventory
Snow_Cannon
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Potion for your player (At the start you can choose only one Potion):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Healing_Potion
(2) Strength_Potion
(3) Magic_Potion
(4) Luck_Elixir
(5) Mermaid_Tears
(6) Ambrosia
->

1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Healing_Potion!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Enter 1 to continue:
1
IceSpells : In Inventory
Healing_Potion
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Type for your player :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1)Warrior
(2)Sorcerer
(3)Paladin
->

1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Warrior!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Type for your player :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1)Gaerdal_Ironhand
(2)Sehanine_Monnbow
(3)Muamman_Duathall
(4)Flandal_Steelskin
(5)Undefeated_Yoj
(6)Eunoia_Cyn
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Gaerdal_Ironhand!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Trait for your player :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1)Strength
(2)Heavy Bones
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Strength!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Weapon for your player (At the start you can choose only one weapon):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Sword
(2) Bow
(3) Scythe
(4) Axe
(5) TSwords
(6) Dagger
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Sword!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Enter 1 to continue:
1
Equip Some Weapon
Sword
Hands Occupied In :0
Ouput I1
Hands Occupied Output : 1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Armor for your player (At the start you can choose only one armor):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Platinum_Shield
(2) Breastplate
(3) Full_Body_Armor
(4) Wizard_Shield
(5) Guardian_Angel
->

1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Platinum_Shield!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Enter 1 to continue:
1
Armors : In Inventory
Platinum_Shield
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Lightning Spell for your player (At the start you can choose only one Lightning Spell):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Lightning_Dagger
(2) Thunder_Blast
(3) Electric_Arrows
(4) Spark_Needles
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Lightning_Dagger!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
spell : LightningSpells@4f3f5b24
Enter 1 to continue:
1
LightningSpells : In Inventory
Lightning_Dagger
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Fire Spell for your player (At the start you can choose only one Fire Spell):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Flame_Tornado
(2) Breath_of_Fire
(3) Heat_Wave
(4) Lava_Comet
(5) Hell_Storm
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Flame_Tornado!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Enter 1 to continue:

1
FireSpells : In Inventory
Flame_Tornado
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Ice Spell for your player (At the start you can choose only one Ice Spell):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Snow_Cannon
(2) Ice_Blade
(3) Frost_Blizzard
(4) Arctic_Storm
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Snow_Cannon!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
-->
1
IceSpells : In Inventory
Snow_Cannon
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Potion for your player (At the start you can choose only one Potion):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Healing_Potion
(2) Strength_Potion
(3) Magic_Potion
(4) Luck_Elixir
(5) Mermaid_Tears
(6) Ambrosia
->

11
->
Enter the ideal choice mentioned

1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Healing_Potion!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Enter 1 to continue:
1
IceSpells : In Inventory
Healing_Potion
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Type for your player :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1)Warrior
(2)Sorcerer
(3)Paladin
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Warrior!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Type for your player :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1)Gaerdal_Ironhand
(2)Sehanine_Monnbow
(3)Muamman_Duathall
(4)Flandal_Steelskin
(5)Undefeated_Yoj
(6)Eunoia_Cyn
->

1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Gaerdal_Ironhand!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Trait for your player :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1)Strength
(2)Heavy Bones
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Strength!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Weapon for your player (At the start you can choose only one weapon):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Sword
(2) Bow
(3) Scythe
(4) Axe
(5) TSwords
(6) Dagger
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Sword!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Enter 1 to continue:

1
Equip Some Weapon
Sword
Hands Occupied In :0
Ouput I1
Hands Occupied Output : 1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Armor for your player (At the start you can choose only one armor):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Platinum_Shield
(2) Breastplate
(3) Full_Body_Armor
(4) Wizard_Shield
(5) Guardian_Angel
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Platinum_Shield!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Enter 1 to continue:
1
Armors : In Inventory
Platinum_Shield
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Lightning Spell for your player (At the start you can choose only one Lightning Spell):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Lightning_Dagger
(2) Thunder_Blast
(3) Electric_Arrows
(4) Spark_Needles
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Lightning_Dagger!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
spell : LightningSpells@15aeb7ab
Enter 1 to continue:
1
LightningSpells : In Inventory
Lightning_Dagger
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Fire Spell for your player (At the start you can choose only one Fire Spell):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Flame_Tornado
(2) Breath_of_Fire
(3) Heat_Wave
(4) Lava_Comet
(5) Hell_Storm
->

1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Flame_Tornado!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Enter 1 to continue:
1
FireSpells : In Inventory
Flame_Tornado
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Ice Spell for your player (At the start you can choose only one Ice Spell):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Snow_Cannon
(2) Ice_Blade
(3) Frost_Blizzard
(4) Arctic_Storm
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Snow_Cannon!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
-->

1
IceSpells : In Inventory
Snow_Cannon
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose a Potion for your player (At the start you can choose only one Potion):
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Healing_Potion
(2) Strength_Potion
(3) Magic_Potion
(4) Luck_Elixir
(5) Mermaid_Tears
(6) Ambrosia
->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You Choose : Healing_Potion!
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Enter 1 to continue:
1
IceSpells : In Inventory
Healing_Potion
Lane size :2
First Border:2
Last Border:5
Lanes Indication :2
Lanes Indication :5
numLanes2
Lane Number :0
i:0j:0
i:0j:1
i:1j:0
i:1j:1
i:2j:0
i:2j:1
i:3j:0
i:3j:1
i:4j:0
i:4j:1
i:5j:0
i:5j:1
i:6j:0
i:6j:1
i:7j:0
i:7j:1
Lane Number :1
i:0j:3
i:0j:4
i:1j:3
i:1j:4
i:2j:3
i:2j:4
i:3j:3
i:3j:4
i:4j:3
i:4j:4
i:5j:3
i:5j:4
i:6j:3
i:6j:4
i:7j:3
i:7j:4
Lane Number :2
Res5
Res5
Res5
Res5
Res5
Res5
Res5
i:0j:6
Res5
i:0j:7
Res5
Res5
Res5
Res5
Res5
Res5
Res5
i:1j:6
Res5
i:1j:7
Res5
Res5
Res5
Res5
Res5
Res5
Res5
i:2j:6
Res5
i:2j:7
Res5
Res5
Res5
Res5
Res5
Res5
Res5
i:3j:6
Res5
i:3j:7
Res5
Res5
Res5
Res5
Res5
Res5
Res5
i:4j:6
Res5
i:4j:7
Res5
Res5
Res5
Res5
Res5
Res5
Res5
i:5j:6
Res5
i:5j:7
Res5
Res5
Res5
Res5
Res5
Res5
Res5
i:6j:6
Res5
i:6j:7
Res5
Res5
Res5
Res5
Res5
Res5
Res5
i:7j:6
Res5
i:7j:7
i:0j:0
i:0j:1
i:1j:0
i:1j:1
i:2j:0
i:2j:1
i:3j:0
i:3j:1
i:4j:0
i:4j:1
i:5j:0
i:5j:1
i:6j:0
i:6j:1
i:7j:0
i:7j:1
i:0j:3
i:0j:4
i:1j:3
i:1j:4
i:2j:3
i:2j:4
i:3j:3
i:3j:4
i:4j:3
i:4j:4
i:5j:3
i:5j:4
i:6j:3
i:6j:4
i:7j:3
i:7j:4
i:0j:6
i:0j:7
i:1j:6
i:1j:7
i:2j:6
i:2j:7
i:3j:6
i:3j:7
i:4j:6
i:4j:7
i:5j:6
i:5j:7
i:6j:6
i:6j:7
i:7j:6
i:7j:7
var size :64
Lane Number :0
































































Lane Number :1
Lane Number :2
Lane Number :3
Land is at positions on the land : 3,0
Land is at positions on the land : 4,0
Land is at positions on the land : 1,0
Land is at positions on the land : 3,0
Land is at positions on the land : 1,0
Land is at positions on the land : 5,1
Land is at positions on the land : 6,0
Land is at positions on the land : 2,0
Land is at positions on the land : 3,1
Land is at positions on the land : 4,1
Land is at positions on the land : 6,1
Land is at positions on the land : 4,0
Land is at positions on the land : 3,0
Land is at positions on the land : 2,0
Land is at positions on the land : 4,1
Land is at positions on the land : 5,0
Land is at positions on the land : 5,1
Land is at positions on the land : 2,1
Land is at positions on the land : 5,1
Land is at positions on the land : 5,1
Land is at positions on the land : 6,0
Land is at positions on the land : 6,1
Land is at positions on the land : 5,0
Land is at positions on the land : 1,0
Land is at positions on the land : 1,1
Land is at positions on the land : 4,1
Land is at positions on the land : 5,0
Land is at positions on the land : 4,1
Land is at positions on the land : 4,0
Land is at positions on the land : 3,1
Land is at positions on the land : 3,0
Land is at positions on the land : 2,0
Land is at positions on the land : 4,0
Land is at positions on the land : 2,1
Land is at positions on the land : 3,0
Land is at positions on the land : 2,0
Land is at positions on the land : 4,1
Land is at positions on the land : 4,1
Land is at positions on the land : 2,1
Land is at positions on the land : 6,1
Land is at positions on the land : 5,1
Land is at positions on the land : 3,1
Land is at positions on the land : 2,1
Land is at positions on the land : 4,1
Land is at positions on the land : 6,1
Land is at positions on the land : 4,1
Land is at positions on the land : 5,1
Land is at positions on the land : 6,0
Land is at positions on the land : 1,1
Land is at positions on the land : 2,0
Land is at positions on the land : 5,0
Land is at positions on the land : 1,1
Land is at positions on the land : 4,0
Land is at positions on the land : 3,0
Land is at positions on the land : 3,0
Land is at positions on the land : 1,1
Land is at positions on the land : 2,0
Land is at positions on the land : 2,1
Land is at positions on the land : 1,0
Land is at positions on the land : 4,0
Land is at positions on the land : 1,1
Land is at positions on the land : 1,0
Land is at positions on the land : 4,0
Land is at positions on the land : 6,1
Land is at positions on the land : 6,3
Land is at positions on the land : 6,4
Land is at positions on the land : 5,3
Land is at positions on the land : 1,3
Land is at positions on the land : 1,3
Land is at positions on the land : 1,4
Land is at positions on the land : 5,3
Land is at positions on the land : 3,4
Land is at positions on the land : 2,3
Land is at positions on the land : 6,3
Land is at positions on the land : 3,4
Land is at positions on the land : 3,3
Land is at positions on the land : 1,4
Land is at positions on the land : 3,3
Land is at positions on the land : 2,4
Land is at positions on the land : 4,3
Land is at positions on the land : 5,4
Land is at positions on the land : 6,3
Land is at positions on the land : 5,4
Land is at positions on the land : 6,4
Land is at positions on the land : 3,3
Land is at positions on the land : 5,4
Land is at positions on the land : 6,4
Land is at positions on the land : 3,4
Land is at positions on the land : 1,3
Land is at positions on the land : 4,3
Land is at positions on the land : 1,4
Land is at positions on the land : 1,3
Land is at positions on the land : 5,3
Land is at positions on the land : 5,3
Land is at positions on the land : 4,3
Land is at positions on the land : 6,4
Land is at positions on the land : 1,3
Land is at positions on the land : 6,4
Land is at positions on the land : 3,4
Land is at positions on the land : 6,4
Land is at positions on the land : 4,3
Land is at positions on the land : 3,3
Land is at positions on the land : 6,3
Land is at positions on the land : 5,4
Land is at positions on the land : 6,3
Land is at positions on the land : 3,3
Land is at positions on the land : 1,4
Land is at positions on the land : 4,4
Land is at positions on the land : 5,4
Land is at positions on the land : 3,4
Land is at positions on the land : 3,4
Land is at positions on the land : 1,3
Land is at positions on the land : 5,4
Land is at positions on the land : 5,3
Land is at positions on the land : 5,4
Land is at positions on the land : 6,3
Land is at positions on the land : 4,3
Land is at positions on the land : 6,3
Land is at positions on the land : 3,3
Land is at positions on the land : 4,4
Land is at positions on the land : 4,4
Land is at positions on the land : 5,4
Land is at positions on the land : 1,3
Land is at positions on the land : 6,4
Land is at positions on the land : 6,3
Land is at positions on the land : 2,4
Land is at positions on the land : 2,3
Land is at positions on the land : 5,4
Land is at positions on the land : 1,7
Land is at positions on the land : 6,6
Land is at positions on the land : 3,6
Land is at positions on the land : 6,6
Land is at positions on the land : 2,6
Land is at positions on the land : 5,7
Land is at positions on the land : 2,7
Land is at positions on the land : 6,7
Land is at positions on the land : 2,6
Land is at positions on the land : 2,7
Land is at positions on the land : 4,7
Land is at positions on the land : 3,7
Land is at positions on the land : 3,6
Land is at positions on the land : 4,7
Land is at positions on the land : 6,7
Land is at positions on the land : 4,6
Land is at positions on the land : 2,7
Land is at positions on the land : 3,7
Land is at positions on the land : 6,7
Land is at positions on the land : 1,6
Land is at positions on the land : 3,6
Land is at positions on the land : 1,6
Land is at positions on the land : 1,7
Land is at positions on the land : 2,6
Land is at positions on the land : 1,6
Land is at positions on the land : 2,6
Land is at positions on the land : 5,6
Land is at positions on the land : 1,7
Land is at positions on the land : 4,6
Land is at positions on the land : 5,6
Land is at positions on the land : 5,6
Land is at positions on the land : 3,7
Land is at positions on the land : 3,6
Land is at positions on the land : 4,6
Land is at positions on the land : 5,6
Land is at positions on the land : 1,7
Land is at positions on the land : 5,7
Land is at positions on the land : 6,6
Land is at positions on the land : 4,7
Land is at positions on the land : 1,6
Land is at positions on the land : 4,7
Land is at positions on the land : 2,6
Land is at positions on the land : 5,7
Land is at positions on the land : 2,7
Land is at positions on the land : 3,6
Land is at positions on the land : 1,7
Land is at positions on the land : 2,7
Land is at positions on the land : 1,7
Land is at positions on the land : 2,7
Land is at positions on the land : 3,7
Land is at positions on the land : 2,6
Land is at positions on the land : 1,6
Land is at positions on the land : 3,7
Land is at positions on the land : 2,6
Land is at positions on the land : 6,7
Land is at positions on the land : 3,7
Land is at positions on the land : 2,6
Land is at positions on the land : 5,6
Land is at positions on the land : 1,6
Land is at positions on the land : 1,7
Land is at positions on the land : 3,6
Land is at positions on the land : 1,6
Land is at positions on the land : 2,6
Land is at positions on the land : 4,7

Market is at positions on the land : 0,0
Market is at positions on the land : 0,1
Market is at positions on the land : 0,3
Market is at positions on the land : 0,4
Market is at positions on the land : 0,6
Market is at positions on the land : 0,7
Market is at positions on the land : 7,0
Market is at positions on the land : 7,1
Market is at positions on the land : 7,4
Market is at positions on the land : 7,3
Market is at positions on the land : 7,6
Market is at positions on the land : 7,7
Market is at positions on the land : 1,0
Market is at positions on the land : 5,3
Market is at positions on the land : 6,7

Cave is at positions on the land : 4,0
Cave is at positions on the land : 2,3
Cave is at positions on the land : 4,6

Bush is at positions on the land : 3,0
Bush is at positions on the land : 4,4
Bush is at positions on the land : 6,6

Koulou is at positions on the land : 1,0
Koulou is at positions on the land : 3,4
Koulou is at positions on the land : 6,6
| G | N | X | N | N | X | N | N | 
| K | L | X | L | L | X | L | L | 
| L | L | X | C | L | X | L | L | 
| B | L | X | L | K | X | L | L | 
| C | L | X | L | B | X | C | L | 
| L | L | X | M | L | X | L | L | 
| L | L | X | L | L | X | B | M | 
| N | N | X | N | N | X | N | N | 
PLease enter the Lane you want to choose to fight the monsters .
-->
1
| G | N | X | N | N | X | N | N | 
| K | L | X | L | L | X | L | L | 
| L | L | X | C | L | X | L | L | 
| B | L | X | L | K | X | L | L | 
| C | L | X | L | B | X | C | L | 
| L | L | X | M | L | X | L | L | 
| L | L | X | L | L | X | B | M | 
| N | H | X | N | N | X | N | N | 
PLease enter the Lane you want to choose to fight the monsters .
-->

1
Checking if the Lane is occupied...
Sir , this Lane is Already occupied , please choose another Lane .
-->
2
Checking if the Lane is occupied...
| G | N | X | N | N | X | N | N | 
| K | L | X | L | L | X | L | L | 
| L | L | X | C | L | X | L | L | 
| B | L | X | L | K | X | L | L | 
| C | L | X | L | B | X | C | L | 
| L | L | X | M | L | X | L | L | 
| L | L | X | L | L | X | B | M | 
| N | H | X | N | W | X | N | N | 
PLease enter the Lane you want to choose to fight the monsters .
-->
3
Checking if the Lane is occupied...
Villain Names : D-Maleficent, Rakkshasass ,BlueEyesWhite ,Igneel, BunsenBurner
Enemies you will be facing : Ereshkigall
Enemies you will be facing : BigBad-Wolf
Enemies you will be facing : D-Maleficent
Number of Demon : 3
Ereshkigall Enters  Lane 1
This Lane Chosen
Ereshkigall Enters  Lane 2
This Lane Choosen
D-Maleficent Enters  Lane 3
This Lane Choosen
Hero 1 move begins :
Villain x : 0, Villain y : 1
Villain x : 0, Villain y : 3
Villain x : 0, Villain y : 6
| N | V | X | E | N | X | S | N | 
| K | L | X | L | L | X | L | L | 
| L | L | X | C | L | X | L | L | 
| B | L | X | L | K | X | L | L | 
| C | L | X | L | B | X | C | L | 
| L | L | X | M | L | X | L | L | 
| L | L | X | L | L | X | B | M | 
| N | H | X | N | W | X | N | G | 
Enter the place you want to move to : W : Up , A : Left , D : Right , S : Down ,TB : Teleport Back, T : Teleport, , Q : Quit , I : Player Info , P: Print Board , K: Inventory Actions,V : Collision Vicinity , SB : Spawn Back To Nexus  
t
Choose Type Of Teleportation you want to use :
(1) Teleportation With Options .
(2) Teleportation Randomly . 
(3) Go Back 
-->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
TELEPORTATION PROGRAM PROCESSING ...........
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Which Hero do you wanna help or transport to ?
(1) Go Back .
(2) Player (2)
(3) Player (3)
-->
2
Size 0 , 0
It enters .
Path Table Empty 
Found W at 7 , 4
Row : 8 Column : 4
Row : 7 Column : 3
Row : 7 Column : 5
Cannot Push this As it will be invalid vicinity 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 7 Column3
Paths you can travel to near Hero 2 are as follows :
 (1)  -->7 , 3
-->
1
x: 7 && y : 3
Something Works !
Size 0 , 0
It enters .
Path Table Empty 
Found H at 7 , 3
Row : 6 Column : 3
Row : 8 Column : 3
Row : 7 Column : 2
Cannot Push this As it will be invalid vicinity 
Row : 7 Column : 4
Row : 6 Column : 2
Cannot Push this As it will be invalid vicinity 
Row : 6 Column : 4
Row : 8 Column : 2
Row : 8 Column : 4
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 7 Column3
 (1) Row : 6 Column3
 (2) Row : 7 Column4
 (3) Row : 6 Column4
It does enter !
You are at the market .Do you want to buy something ?
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You have arrived at the Market . Do you want to Enter ?
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Yes
(2) No
--> 
2
Villain x : 0, Villain y : 1
Villain x : 0, Villain y : 3
Villain x : 0, Villain y : 6
| N | V | X | E | N | X | S | N | 
| K | L | X | L | L | X | L | L | 
| L | L | X | C | L | X | L | L | 
| B | L | X | L | K | X | L | L | 
| C | L | X | L | B | X | C | L | 
| L | L | X | M | L | X | L | L | 
| L | L | X | L | L | X | B | M | 
| N | N | X | H | W | X | N | G | 
  
Hero List Size :3
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Hero 2 move begins :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Villain x : 0, Villain y : 1
Villain x : 0, Villain y : 3
Villain x : 0, Villain y : 6
| N | V | X | E | N | X | S | N | 
| K | L | X | L | L | X | L | L | 
| L | L | X | C | L | X | L | L | 
| B | L | X | L | K | X | L | L | 
| C | L | X | L | B | X | C | L | 
| L | L | X | M | L | X | L | L | 
| L | L | X | L | L | X | B | M | 
| N | N | X | H | W | X | N | G | 
Enter the place you want to move to : W : Up , A : Left , D : Right , S : Down ,TB : Teleport Back, T : Teleport, , Q : Quit , I : Player Info , P: Print Board , K: Inventory Actions,V : Collision Vicinity , SB : Spawn Back To Nexus  
t
Choose Type Of Teleportation you want to use :
(1) Teleportation With Options .
(2) Teleportation Randomly . 
(3) Go Back 
-->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
TELEPORTATION PROGRAM PROCESSING ...........
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Which Hero do you wanna help or transport to ?
(1) Player (1)
(2) Go Back. 
(3) Player (3)
-->
3
Size 0 , 0
Size 0 , 0
It enters .
Path Table Empty 
Found G at 7 , 7
Row : 8 Column : 7
Row : 7 Column : 6
Row : 7 Column : 8
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 7 Column6
Paths you can travel to near Hero 3 are as follows :
 (1)  -->7 , 6
-->
1
x: 7 && y : 6
Something Works !
Path Table not Empty!
Size 2 , 2
It enters .
Path Table not Empty!
Path Table not Empty!
Size 0 , 0
Path Table Empty 
Found W at 7 , 6
Row : 6 Column : 6
Row : 8 Column : 6
Row : 7 Column : 5
Cannot Push this As it will be invalid vicinity 
Row : 7 Column : 7
Row : 6 Column : 5
Cannot Push this As it will be invalid vicinity 
Row : 6 Column : 7
Row : 8 Column : 5
Row : 8 Column : 7
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 7 Column6
 (1) Row : 6 Column6
 (2) Row : 7 Column7
 (3) Row : 6 Column7
It does enter !
You are at the market .Do you want to buy something ?
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You have arrived at the Market . Do you want to Enter ?
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Yes
(2) No
--> 
2
Villain x : 0, Villain y : 1
Villain x : 0, Villain y : 3
Villain x : 0, Villain y : 6
| N | V | X | E | N | X | S | N | 
| K | L | X | L | L | X | L | L | 
| L | L | X | C | L | X | L | L | 
| B | L | X | L | K | X | L | L | 
| C | L | X | L | B | X | C | L | 
| L | L | X | M | L | X | L | L | 
| L | L | X | L | L | X | B | M | 
| N | N | X | H | N | X | W | G | 
  
Hero List Size :3
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Hero 3 move begins :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Villain x : 0, Villain y : 1
Villain x : 0, Villain y : 3
Villain x : 0, Villain y : 6
| N | V | X | E | N | X | S | N | 
| K | L | X | L | L | X | L | L | 
| L | L | X | C | L | X | L | L | 
| B | L | X | L | K | X | L | L | 
| C | L | X | L | B | X | C | L | 
| L | L | X | M | L | X | L | L | 
| L | L | X | L | L | X | B | M | 
| N | N | X | H | N | X | W | G | 
Enter the place you want to move to : W : Up , A : Left , D : Right , S : Down ,TB : Teleport Back, T : Teleport, , Q : Quit , I : Player Info , P: Print Board , K: Inventory Actions,V : Collision Vicinity , SB : Spawn Back To Nexus 
t
Choose Type Of Teleportation you want to use :
(1) Teleportation With Options .
(2) Teleportation Randomly . 
(3) Go Back 
-->
1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
TELEPORTATION PROGRAM PROCESSING ...........
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Which Hero do you wanna help or transport to ?
(1) Player (1)
(2)  Player (2) 
(3) Go Back
-->
1
Size 0 , 0
Size 0 , 0
It enters .
Path Table Empty 
Found H at 7 , 3
Row : 8 Column : 3
Row : 7 Column : 2
Cannot Push this As it will be invalid vicinity 
Row : 7 Column : 4
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 7 Column4
Paths you can travel to near Hero 1 are as follows :
 (1)  -->7 , 4
-->
1
x: 7 && y : 4
Something Works !
Path Table not Empty!
Size 2 , 2
It enters .
Path Table not Empty!
Path Table not Empty!
Size 0 , 0
Path Table Empty 
Found G at 7 , 4
Row : 6 Column : 4
Row : 8 Column : 4
Row : 7 Column : 3
Row : 7 Column : 5
Cannot Push this As it will be invalid vicinity 
Row : 6 Column : 3
Row : 6 Column : 5
Cannot Push this As it will be invalid vicinity 
Row : 8 Column : 3
Row : 8 Column : 5
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 7 Column4
 (1) Row : 6 Column4
 (2) Row : 7 Column3
 (3) Row : 6 Column3
It does enter !
You are at the market .Do you want to buy something ?
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You have arrived at the Market . Do you want to Enter ?
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Yes
(2) No
--> 
2
Villain x : 0, Villain y : 1
Villain x : 0, Villain y : 3
Villain x : 0, Villain y : 6
| N | V | X | E | N | X | S | N | 
| K | L | X | L | L | X | L | L | 
| L | L | X | C | L | X | L | L | 
| B | L | X | L | K | X | L | L | 
| C | L | X | L | B | X | C | L | 
| L | L | X | M | L | X | L | L | 
| L | L | X | L | L | X | B | M | 
| N | N | X | H | G | X | W | N | 
  
Hero List Size :3
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Monster move begins :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
x: 1 && y : 1
It Enters
Sound should start!
Villain :0 has moved to coordinates  : 1,1 and the number of villains right now is : 0
 
Something Works !
Path Table not Empty!
Size 2 , 2
Path Table not Empty!
Path Table not Empty!
Size 0 , 0
It enters .
Path Table Empty 
Found H at 7 , 3
Row : 6 Column : 3
Row : 8 Column : 3
Row : 7 Column : 2
Cannot Push this As it will be invalid vicinity 
Row : 7 Column : 4
Row : 6 Column : 2
Cannot Push this As it will be invalid vicinity 
Row : 6 Column : 4
Row : 8 Column : 2
Row : 8 Column : 4
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 7 Column3
 (1) Row : 6 Column3
 (2) Row : 7 Column4
 (3) Row : 6 Column4
It does enter !
x: 1 && y : 3
It Enters
Sound should start!
Villain :1 has moved to coordinates  : 1,3 and the number of villains right now is : 0
 
Something Works !
Path Table not Empty!
Size 2 , 2
It enters .
Path Table not Empty!
Path Table not Empty!
Size 0 , 0
Path Table Empty 
Found W at 7 , 6
Row : 6 Column : 6
Row : 8 Column : 6
Row : 7 Column : 5
Cannot Push this As it will be invalid vicinity 
Row : 7 Column : 7
Row : 6 Column : 5
Cannot Push this As it will be invalid vicinity 
Row : 6 Column : 7
Row : 8 Column : 5
Row : 8 Column : 7
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 7 Column6
 (1) Row : 6 Column6
 (2) Row : 7 Column7
 (3) Row : 6 Column7
It does enter !
Start Again
No Man's Land . Go Somewhere Else.
No Man's Land . Go Somewhere Else.
x: 1 && y : 6
It Enters
Sound should start!
Villain :2 has moved to coordinates  : 1,6 and the number of villains right now is : 0
 
 
Something Works !
Path Table not Empty!
Size 2 , 2
It enters .
Path Table not Empty!
Path Table not Empty!
Size 0 , 0
Path Table Empty 
Found G at 7 , 4
Row : 6 Column : 4
Row : 8 Column : 4
Row : 7 Column : 3
Row : 7 Column : 5
Cannot Push this As it will be invalid vicinity 
Row : 6 Column : 3
Row : 6 Column : 5
Cannot Push this As it will be invalid vicinity 
Row : 8 Column : 3
Row : 8 Column : 5
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 7 Column4
 (1) Row : 6 Column4
 (2) Row : 7 Column3
 (3) Row : 6 Column3
It does enter !
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Turn 1 Begins !!!!! 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Hero 1 move begins 
Villain x : 1, Villain y : 1
Villain x : 1, Villain y : 3
Villain x : 1, Villain y : 6
| N | N | X | N | N | X | N | N | 
| K | V | X | E | L | X | S | L | 
| L | L | X | C | L | X | L | L | 
| B | L | X | L | K | X | L | L | 
| C | L | X | L | B | X | C | L | 
| L | L | X | M | L | X | L | L | 
| L | L | X | L | L | X | B | M | 
| N | N | X | H | G | X | W | N | 
Enter the place you want to move to : W : Up , A : Left , D : Right , S : Down ,TB : Teleport Back, T : Teleport, , Q : Quit , I : Player Info , P: Print Board , K: Inventory Actions,V : Collision Vicinity , SB : Spawn Back To Nexus  


CASE II : Hero Death : 
| N | N | X | N | N | X | N | N | 
| L | L | X | K | L | X | L | L | 
| V | M | X | E | M | X | L | S | 
| L | C | X | L | L | X | L | B | 
| B | H | X | L | W | X | L | L | 
| K | L | X | C | L | X | G | L | 
| L | L | X | L | L | X | M | L | 
| N | N | X | N | N | X | N | N | 
  
Hero List Size :3
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Monster move begins :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
x: 3 && y : 0
It Enters
Sound should start!
Villain :0 has moved to coordinates  : 3,0 and the number of villains right now is : 0
 
Something Works !
Path Table not Empty!
Size 3 , 3
Path Table not Empty!
Path Table not Empty!
Size 0 , 0
It enters .
Path Table Empty 
Found H at 4 , 1
Row : 3 Column : 1
Row : 5 Column : 1
Row : 4 Column : 0
Row : 4 Column : 2
Cannot Push this As it will be invalid vicinity 
Row : 3 Column : 0
Row : 3 Column : 2
Cannot Push this As it will be invalid vicinity 
Row : 5 Column : 0
Row : 5 Column : 2
Cannot Push this As it will be invalid vicinity 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 4 Column1
 (1) Row : 3 Column1
 (2) Row : 5 Column1
 (3) Row : 4 Column0
 (4) Row : 3 Column0
 (5) Row : 5 Column0
It does enter !
Battle might Happen .
--->
1
Hero Identity : 0 Hero List Size : 3
Hero Level : 1
It Enters here .
It Enters here H.
You have encountered an Enemy , In order to survive you have to fight it.
Number of Heroes 3
Villain Names : Merrshaullk, Melchiresas ,Kas-Ethelinh ,Alexstraszan, Merrshaullk
Enemies you will be facing : Rakkshasass
Enemies you will be facing : DocOck
Enemies you will be facing : Exodia
Enemies you will be facing : Aasterinian
Enemies you will be facing : BigBad-Wolf
Enemies you will be facing : Andrealphus
Heroes@49c2faae
Heroes@20ad9418
Heroes@31cefde0
Hero Identity : 0 Hero List Size : 3
Hero Identity : 0 Hero List Size : 3
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Rakkshasass
 HP: 100 / 100
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Gaerdal_Ironhand
 HP: 100 / 100
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose am Action to perform :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Attack (with Weapon)
(2) Attack (with Spell)
(3) Attack (with Hand)
(4) Consume Potion
(5) See Inventory(Weapons, Armors, Spells)
(6) Drop To Inventory(Weapon)
(7) Equip from Inventory(Weapon)
(8) Run From Battle
(9) Equip from Inventory(Armor)
(10) Drop To Inventory(Armor)
(11) Equip from Inventory(Spell)
(12) Drop To Inventory(Spell)
(13) Equip from Inventory(Potion)
(14) Drop To Inventory(Potion)
(15) Check Info OF Heroes
(16) Check Info OF Villains
Enter your choice
1
28
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
WAR
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Damage :5
You inflicted 5 damage on the Rakkshasass .
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
The enemy Rakkshasass inflicted  20 on you .
Hero Identity : 0 Hero List Size : 3
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Rakkshasass
 HP: 95 / 100
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Gaerdal_Ironhand
 HP: 80 / 100
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose am Action to perform :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Attack (with Weapon)
(2) Attack (with Spell)
(3) Attack (with Hand)
(4) Consume Potion
(5) See Inventory(Weapons, Armors, Spells)
(6) Drop To Inventory(Weapon)
(7) Equip from Inventory(Weapon)
(8) Run From Battle
(9) Equip from Inventory(Armor)
(10) Drop To Inventory(Armor)
(11) Equip from Inventory(Spell)
(12) Drop To Inventory(Spell)
(13) Equip from Inventory(Potion)
(14) Drop To Inventory(Potion)
(15) Check Info OF Heroes
(16) Check Info OF Villains
Enter your choice
1
25
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
WAR
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Damage :1
You inflicted 1 damage on the Rakkshasass .
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
The enemy Rakkshasass inflicted  33 on you .
Hero Identity : 0 Hero List Size : 3
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Rakkshasass
 HP: 94 / 100
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Gaerdal_Ironhand
 HP: 47 / 100
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose am Action to perform :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Attack (with Weapon)
(2) Attack (with Spell)
(3) Attack (with Hand)
(4) Consume Potion
(5) See Inventory(Weapons, Armors, Spells)
(6) Drop To Inventory(Weapon)
(7) Equip from Inventory(Weapon)
(8) Run From Battle
(9) Equip from Inventory(Armor)
(10) Drop To Inventory(Armor)
(11) Equip from Inventory(Spell)
(12) Drop To Inventory(Spell)
(13) Equip from Inventory(Potion)
(14) Drop To Inventory(Potion)
(15) Check Info OF Heroes
(16) Check Info OF Villains
Enter your choice
1
34
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
WAR
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Damage :5
You inflicted 5 damage on the Rakkshasass .
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
The enemy Rakkshasass inflicted  37 on you .
Hero Identity : 0 Hero List Size : 3
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Rakkshasass
 HP: 89 / 100
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Gaerdal_Ironhand
 HP: 10 / 100
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose am Action to perform :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Attack (with Weapon)
(2) Attack (with Spell)
(3) Attack (with Hand)
(4) Consume Potion
(5) See Inventory(Weapons, Armors, Spells)
(6) Drop To Inventory(Weapon)
(7) Equip from Inventory(Weapon)
(8) Run From Battle
(9) Equip from Inventory(Armor)
(10) Drop To Inventory(Armor)
(11) Equip from Inventory(Spell)
(12) Drop To Inventory(Spell)
(13) Equip from Inventory(Potion)
(14) Drop To Inventory(Potion)
(15) Check Info OF Heroes
(16) Check Info OF Villains
Enter your choice
1
62
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
WAR
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Damage :55
You inflicted 55 damage on the Rakkshasass .
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
The enemy Rakkshasass inflicted  27 on you .
Player HP :-17
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
May your soul rest in Peace .
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You earned 7 XP on your journey to defeat monsters 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Thanks for playing this , do try again for enjoying more of the adventure .
Your Game Ended. Sorry Try Again Next Time.
Player Gaerdal_Ironhandhas fainted . Now it's up on the remaining Heroes to defend your Honor.
 ( 0 ) -->Gaerdal_Ironhand are alive .
 ( 1 ) -->Gaerdal_Ironhand are alive .
 Hero that died : 0
Villain x : 3, Villain y : 0
Villain x : 2, Villain y : 3
Villain x : 2, Villain y : 7
| N | N | X | N | N | X | N | N | 
| L | L | X | K | L | X | L | L | 
| L | M | X | E | M | X | L | S | 
| V | C | X | L | L | X | L | B | 
| B | L | X | L | W | X | L | L | 
| K | L | X | C | L | X | G | L | 
| L | L | X | L | L | X | M | L | 
| N | N | X | N | N | X | N | N | 
Hero List Size 2
Villain x : 3, Villain y : 0
Villain x : 2, Villain y : 3
Villain x : 2, Villain y : 7
| N | N | X | N | N | X | N | N | 
| L | L | X | K | L | X | L | L | 
| L | M | X | E | M | X | L | S | 
| V | C | X | L | L | X | L | B | 
| B | L | X | L | W | X | L | L | 
| K | L | X | C | L | X | G | L | 
| L | L | X | L | L | X | M | L | 
| N | N | X | N | N | X | N | N | 
You were previously at the Bush .Your dexterity will return to normal .
Enter the place you want to move to : W : Up , A : Left , D : Right , S : Down ,TB : Teleport Back, T : Teleport, , Q : Quit , I : Player Info , P: Print Board , K: Inventory Actions,V : Collision Vicinity , SB : Spawn Back To Nexus  


Case III : Vilain Death :



| N | N | X | N | N | X | N | N | 
| L | L | X | L | L | X | L | M | 
| L | V | X | L | E | X | L | S | 
| M | L | X | L | C | X | L | B | 
| H | K | X | W | B | X | L | L | 
| B | C | X | L | M | X | L | G | 
| L | L | X | K | L | X | L | C | 
| N | N | X | N | N | X | N | N | 
Enter the place you want to move to : W : Up , A : Left , D : Right , S : Down ,TB : Teleport Back, T : Teleport, , Q : Quit , I : Player Info , P: Print Board , K: Inventory Actions,V : Collision Vicinity , SB : Spawn Back To Nexus 
a
x: 5 && y : 6
It Enters
Sound should start!
 
Something Works !
Path Table not Empty!
Size 3 , 3
It enters .
Path Table not Empty!
Path Table not Empty!
Size 0 , 0
Path Table Empty 
Found G at 5 , 6
Row : 4 Column : 6
Row : 6 Column : 6
Row : 5 Column : 5
Cannot Push this As it will be invalid vicinity 
Row : 5 Column : 7
Row : 4 Column : 5
Cannot Push this As it will be invalid vicinity 
Row : 4 Column : 7
Row : 6 Column : 5
Cannot Push this As it will be invalid vicinity 
Row : 6 Column : 7
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 5 Column6
 (1) Row : 4 Column6
 (2) Row : 6 Column6
 (3) Row : 5 Column7
 (4) Row : 4 Column7
 (5) Row : 6 Column7
It does enter !
You are on the common Land .
You are on the common Land .
You are on the common Land .
You are on the common Land .
You are on the common Land .
You are on the common Land .
Villain x : 2, Villain y : 1
Villain x : 2, Villain y : 4
Villain x : 2, Villain y : 7
| N | N | X | N | N | X | N | N | 
| L | L | X | L | L | X | L | M | 
| L | V | X | L | E | X | L | S | 
| M | L | X | L | C | X | L | B | 
| H | K | X | W | B | X | L | L | 
| B | C | X | L | M | X | G | L | 
| L | L | X | K | L | X | L | C | 
| N | N | X | N | N | X | N | N | 
  
Hero List Size :3
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Monster move begins :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
x: 3 && y : 1
It Enters
Sound should start!
Villain :0 has moved to coordinates  : 3,1 and the number of villains right now is : 0
 
Something Works !
Path Table not Empty!
Size 3 , 3
Path Table not Empty!
Path Table not Empty!
Size 0 , 0
It enters .
Path Table Empty 
Found H at 4 , 0
Row : 3 Column : 0
Row : 5 Column : 0
Row : 4 Column : -1
Row : 4 Column : 1
Row : 3 Column : -1
Row : 3 Column : 1
Row : 5 Column : -1
Row : 5 Column : 1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 4 Column0
 (1) Row : 3 Column0
 (2) Row : 5 Column0
 (3) Row : 4 Column1
 (4) Row : 3 Column1
 (5) Row : 5 Column1
It does enter !
Battle might Happen .
--->
1
Hero Identity : 0 Hero List Size : 3
Hero Level : 1
It Enters here .
It Enters here H.
You have encountered an Enemy , In order to survive you have to fight it.
Number of Heroes 3
Villain Names : Cyrrollalee, Igneel ,Chiang-shih ,Merrshaullk, Brandobaris
Enemies you will be facing : Blinky
Enemies you will be facing : Blinky
Enemies you will be facing : Kiaransalee
Enemies you will be facing : Jormunngand
Enemies you will be facing : Andrealphus
Enemies you will be facing : Chronepsish
Heroes@49c2faae
Heroes@20ad9418
Heroes@31cefde0
Hero Identity : 0 Hero List Size : 3
Hero Identity : 0 Hero List Size : 3
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Blinky
 HP: 100 / 100
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Gaerdal_Ironhand
 HP: 100 / 100
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Choose am Action to perform :
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
(1) Attack (with Weapon)
(2) Attack (with Spell)
(3) Attack (with Hand)
(4) Consume Potion
(5) See Inventory(Weapons, Armors, Spells)
(6) Drop To Inventory(Weapon)
(7) Equip from Inventory(Weapon)
(8) Run From Battle
(9) Equip from Inventory(Armor)
(10) Drop To Inventory(Armor)
(11) Equip from Inventory(Spell)
(12) Drop To Inventory(Spell)
(13) Equip from Inventory(Potion)
(14) Drop To Inventory(Potion)
(15) Check Info OF Heroes
(16) Check Info OF Villains
Enter your choice
3
948
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
WAR
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Damage :942
You inflicted 942 damage on the Blinky .
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
The enemy Blinky inflicted  22 on you .
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You defeated the Blinky !
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
You earned the 1 XP!
You collect 57 gold from theBlinky's corpse !
Villain List Size :0
Symbol :V
Villain Dead Symbol : V
Hero Symbol :H
Something Works !
Path Table not Empty!
Size 3 , 3
Path Table not Empty!
Path Table not Empty!
Size 0 , 0
It enters .
Path Table Empty 
Found H at 4 , 0
Row : 3 Column : 0
Row : 5 Column : 0
Row : 4 Column : -1
Row : 4 Column : 1
Row : 3 Column : -1
Row : 3 Column : 1
Row : 5 Column : -1
Row : 5 Column : 1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 4 Column0
 (1) Row : 3 Column0
 (2) Row : 5 Column0
 (3) Row : 4 Column1
 (4) Row : 3 Column1
 (5) Row : 5 Column1
Villain x : 16, Villain y : 16
Villain x : 2, Villain y : 4
Villain x : 2, Villain y : 7
| N | N | X | N | N | X | N | N | 
| L | L | X | L | L | X | L | M | 
| L | L | X | L | E | X | L | S | 
| M | L | X | L | C | X | L | B | 
| H | K | X | W | B | X | L | L | 
| B | C | X | L | M | X | G | L | 
| L | L | X | K | L | X | L | C | 
| N | N | X | N | N | X | N | N | 
Something Works !
Path Table not Empty!
Size 3 , 3
It enters .
Path Table not Empty!
Path Table not Empty!
Size 0 , 0
Path Table Empty 
Found W at 4 , 3
Row : 3 Column : 3
Row : 5 Column : 3
Row : 4 Column : 2
Cannot Push this As it will be invalid vicinity 
Row : 4 Column : 4
Row : 3 Column : 2
Cannot Push this As it will be invalid vicinity 
Row : 3 Column : 4
Row : 5 Column : 2
Cannot Push this As it will be invalid vicinity 
Row : 5 Column : 4
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 4 Column3
 (1) Row : 3 Column3
 (2) Row : 5 Column3
 (3) Row : 4 Column4
 (4) Row : 3 Column4
 (5) Row : 5 Column4
Something Works !
Path Table not Empty!
Size 3 , 3
It enters .
Path Table not Empty!
Path Table not Empty!
Size 0 , 0
Path Table Empty 
Found G at 5 , 6
Row : 4 Column : 6
Row : 6 Column : 6
Row : 5 Column : 5
Cannot Push this As it will be invalid vicinity 
Row : 5 Column : 7
Row : 4 Column : 5
Cannot Push this As it will be invalid vicinity 
Row : 4 Column : 7
Row : 6 Column : 5
Cannot Push this As it will be invalid vicinity 
Row : 6 Column : 7
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 5 Column6
 (1) Row : 4 Column6
 (2) Row : 6 Column6
 (3) Row : 5 Column7
 (4) Row : 4 Column7
 (5) Row : 6 Column7
Something Works !
Path Table not Empty!
Size 3 , 3
Path Table not Empty!
Path Table not Empty!
Size 0 , 0
It enters .
Path Table Empty 
Found H at 4 , 0
Row : 3 Column : 0
Row : 5 Column : 0
Row : 4 Column : -1
Row : 4 Column : 1
Row : 3 Column : -1
Row : 3 Column : 1
Row : 5 Column : -1
Row : 5 Column : 1
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
Your Vicinity Paths are as follows : 
 --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  --  -- 
 (0) Row : 4 Column0
 (1) Row : 3 Column0
 (2) Row : 5 Column0
 (3) Row : 4 Column1
 (4) Row : 3 Column1
 (5) Row : 5 Column1
Villain x : 16, Villain y : 16
Villain x : 2, Villain y : 4
Villain x : 2, Villain y : 7
| N | N | X | N | N | X | N | N | 
| L | L | X | L | L | X | L | M | 
| L | L | X | L | E | X | L | S | 
| M | L | X | L | C | X | L | B | 
| H | K | X | W | B | X | L | L | 
| B | C | X | L | M | X | G | L | 
| L | L | X | K | L | X | L | C | 
| N | N | X | N | N | X | N | N | 
Villain x : 16, Villain y : 16
Villain x : 2, Villain y : 4
Villain x : 2, Villain y : 7
| N | N | X | N | N | X | N | N | 
| L | L | X | L | L | X | L | M | 
| L | L | X | L | E | X | L | S | 
| M | L | X | L | C | X | L | B | 
| H | K | X | W | B | X | L | L | 
| B | C | X | L | M | X | G | L | 
| L | L | X | K | L | X | L | C | 
| N | N | X | N | N | X | N | N | 
Villain List Size 0
Villain x : 16, Villain y : 16
Villain x : 2, Villain y : 4
Villain x : 2, Villain y : 7
| N | N | X | N | N | X | N | N | 
| L | L | X | L | L | X | L | M | 
| L | L | X | L | E | X | L | S | 
| M | L | X | L | C | X | L | B | 
| H | K | X | W | B | X | L | L | 
| B | C | X | L | M | X | G | L | 
| L | L | X | K | L | X | L | C | 
| N | N | X | N | N | X | N | N | 
Enter the place you want to move to : W : Up , A : Left , D : Right , S : Down ,TB : Teleport Back, T : Teleport, , Q : Quit , I : Player Info , P: Print Board , K: Inventory Actions,V : Collision Vicinity , SB : Spawn Back To Nexus  

