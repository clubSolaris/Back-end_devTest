# Developer Coding Test

## Bases
Be sure to read all of this document carefully, and follow the guidelines within.
Problem Description

ZSSN (Zombie Survival Social Network). The world as we know it has fallen into an apocalyptic scenario. A laboratory-made virus is transforming human beings and animals into zombies, hungry for fresh flesh.

You, as a zombie resistance member (and the last survivor who knows how to code), was designated to develop a system to share resources between non-infected humans.
Requirements

You will develop a REST API (yes, we care about architecture design even in the midst of a zombie apocalypse!), which will store information about the survivors, as well as the resources they own.

In order to accomplish this, the API must fulfill the following use cases:

    - Add survivors to the database
    - A survivor must have a name, age, gender and last location (latitude, longitude).
    - A survivor also has an inventory of resources of their own property (which you need to declare when upon the registration of the survivor).
    - Update survivor location
    - A survivor must have the ability to update their last location, storing the new latitude/longitude pair in the base (need to track locations, showing last one as property of the survivor).
    - Flag survivor as infected
    - In a chaotic situation like that, it's inevitable that a survivor may get contaminated by the virus. When this happens, we need to flag the survivor as infected.
    - An infected survivor cannot trade with others, can't access/manipulate their inventory, nor be listed in the reports (infected people are kinda dead anyway, see the item on reports below).
    - A survivor is marked as infected when at least three other near survivors report their contamination.
    - When a survivor is infected, their inventory items become inaccessible (they cannot trade with others).
    - Survivors cannot Add/Remove items from inventory
    - Their belongings must be declared when they are first registered in the system. After that they can only change their inventory by means of trading with other survivors.
    - The items allowed in the inventory are described above in the first feature.

Trade items:

    - Survivors can trade items among themselves.
    - To do that, they must respect the price table below, where the value of an item is described in terms of points.
    - Both sides of the trade should offer the same amount of points. For example, 1 Water and 1 Medication (1 x 4 + 1 x 2) is worth 6 ammunition (6 x 1) or 2 Food items (2 x 3).
    - The trades themselves need to be stored to know who trades what, but the items must be transferred from one survivor to the other.

 	
| Item | Points |
| ------ | ------ |
| 1 Water | 4 points |
| 1 Food | 3 points |
| 1 Medication | 2 points |
| 1 Ammunition | 1 point |
 	
 	
 	
 	

## Reports

The API must offer the following reports:

    - Percentage of infected survivors.
    - Percentage of non-infected survivors.
    - Average amount of each kind of resource by survivor (e.g. 5 waters per survivor)
    - Points lost because of infected survivors.
    - Small website 

This website must be ableto show the results of reports as tables and a way to select update interval of the tables
Notes

    - Please use one of the following languages/frameworks: PHP, Javascript
    - No authentication is needed (it's a zombie apocalypse, no one will try to hack a system while running from a horde of zombies);
    - We still care about proper programming and architecture techniques, you must showcase that you're worthy of surving the zombie apocalypse through the sheer strength of your skills;
    - Don't forget to make at least a minimal documentation of the API endpoints and how to use them;
    - You must write at least some automated tests;
    - From the problem description above you can either do a very bare bones solution or add optional features that are not described. Use your time wisely; the absolute optimal solution might take too long to be effective in the apocalypse, so you must come up with the best possible solution that will hold up within the least ammount of time and still be able to showcase your skills in order to prove your worth.
    - Write concise and clear commit messages, splitting your changes in little pieces.

