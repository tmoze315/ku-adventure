---
description: 'You''ve got a lot of stuff, now what do you do with it?'
---

# Equipment & Backpack

After you `-loot` your treasure, you can either wear it or put it in your backpack. To view items, you can use the basic command `-backpack` or you can change up the game and really put some effort into your gear! Use any of the following commands to interact with your backpack and items:

* `-backpack eset` - Equip all pieces of a set that you are able to equip.
* `-ebackpack` accepts all the same arguments as `-backpack` but will only show items you can equip.
*  `-mysets` - Show all available sets and how many pieces you own.
*  `-cbackpack`
*  `-cbackpack show` - Show items in your backpack that match the specified query.
*  `-cbackpack sell` - Sell items in your backpack that match the specified query.
* `-cbackpack disassemble` - Disassemble items in your backpack that match the specified query.
* `-unequip` accepts `all` as an argument, which will unequip all equipped gear.
* `-backpack disassemble` accepts rarities as an argument, which will dismantle all items in that rarity.

If you're like to get more complex about your queries into your backpack, use the following information:

* `-cbackpack show --equip --lvl >50`
  * Will show only items that you are able to equip which have level higher than 50.
* `-cbackpack sell --slot head charm --rarity legendary ascended --no-match celestial --icase --lvl >50 <100`
  * Will sell all legendary and ascended items in the head and charm slot that do not have the word "celestial" in them and that their level is between 51 and 99
* `-cbackpack show --except --str >50`
  * Will show all items that have less than 50 str points
* `-cbackpack show --except --no-match celestial`
  * Will Show every item that has "celestial" in the name \(Case sensitive as `--icase` was not used\)



**--slot** - Accepts multiple slots \(use quotes if there are spaces in a slot name\).  
**--rarity** - Accepts multiple rarities.  
**--set** - Accepts multiple sets \(use quotes if there are spaces in the set name\).  
**--equip** - If used will only show equippable items.  
**--diff** - If used will show the stat delta compared to what you currently have equipped \(Only works on `-cbackpack show`\).  
**--except** - If used will show everything that does not match the specified query.  
**--match** - Accepts a string, no quotes are needed. Will attempt to match items to this string.  
**--no-match** - Opposite of `--match`  
**--icase** - If `--match` or `--no-match` and `--icase` are used, matches will not be case sensitive.  


\#\#\#\#\#\#For the following arguments:  


* These arguments accept 1 or 2 numbers. If 1 is passed it is treated as an equal match, if 2 then it is a range. 
  * **--str**
  * **--int**
  * **--cha**
  * **--luc**
  * **--dex**
  * **--lvl**
  * **--deg** \(Only works on `-cbackpack show`\)

