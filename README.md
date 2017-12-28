# STV-The-Long-Journey
Overview of the Project:

-This is a fan project to develop a roster management game based on the show Star Trek Voyager. This is not intended to be sold and should not be considered to be sold in any fashion. My primary goal in making this is to under take a project to expand my skills as a programmer, expand my expierence with python speccifically, and to learn how to use Github. 

What is a roster Management game?

-Just like the name implies, instead of controlling speccific assets you manage those assets by roster. In the case of the plans for this game, the assets to be managed are the crew of the USS Voyager and you manage them by assigning them to missions and departments. So you can assign Ensign Kim to operations, or you can assign him to Sick bay. He will perform better in some departments then others based on his individual traits and skills so you will want to maximize his contributions to the ship by assigning him to departments and missions that suite his skills. However, there could be times where he is the best option for a department or mission that he is only moderatly skilled in due to mission demands or injuried/killed crew members. 

Major points about the game?

-The Long Journey is intended to be a largely open ended roster management game that starts with the USS Voyager and the Maquis ship, The Val Jean, having been pulled across the galaxy into the Delta quadrant. From this point onwards your decisions will effect how the ship suffers or prospers. Will you integrate the Maquis crew into your own? Or will you execute them all? Will you allie with the Kazon or declare war on them? These are all options that will be availible to the player. The player's choices will affect what crew member live and die while also having the ability to recruit new crew members during the process of a game.

How do you win the game?

-By default the game will operate on the 'The Long Journey' Mission. Every day of in-game time that this mission is being under taken, the ship will be recorded as having traveled 100 light years. When this mission has totaled 70,000 light years traveled, the player will win the game. 
- Under taking other missions that require travel time do not add to this total.
- possibility of one-time events adding a set amount to the distance traveled. (Ex: Kes throwing voyager 10k light years).

Development notes: This section will be any accumulated notes regarding the game.
==================================================================================================================================

Star Trek Voyager The Long Journey: You would take on the role of Captain Janeway as she attempts to lead the USS Voyager home from the delta quadrant, a journy they by all estimates will take over 75 years. You must pick the right people for the right jobs to maximize your chances not only of survival, but also in gathering supplies to maintain your ship and crew, but also in obtaining additional tech to aide you in your journey. The game itself would would be a roster management game with minimal graphics. The over all idea is you would have a roster of crew members. Each crew member would have their respective stats including race, gender, rank, mission role, science rating, engineering rating, ranged combat rating, hand to hand combat rating, regeneration, stress, fortitutde, mental fortitude and morale. These stats would be used in under taking various missions and assignments. 

So you would have several screens that would allow you to view damage to the ship, details about upgrades to the ship, view crew roster, department assignments, and missions assignments. 

list of screens accessible to the player:
Captains Command center: the CCC provides the overall view of the ship status and crew status. Displaying over all crew morale status.
- crew roster: A complete listing of the ships crew, can be sorted alphabetically, by species, by department, or by rank. Would be able to assign crew member to department from this screen. The department that the crew member is assigned to will be their default posting after they return from an away mission or after medical treatment.
- crew member profile: A detailed view of an individual crew member including their stats, and assembled baground/bio.
- department reports: detailed view of status of the ship by department. Would include information regarding department efficency and status as well as any notes regarding supply short falls and their effects. Would also be able to pull up a list of crew members assigned to this department.
- away team report: Display the current status of any currently active away missions.
- tactical display: would display current status of the ship and it's weapon system. Display would include a wire frame display of the ship with sections picked out in color to denote damage levels. Green would indicate normal operation and no damage. teal would indicate up to 15% damage to that area, but otherwise operational. blue would indicate damge more then 15% and up to 35% with up to 25% impaired functionality. Blue would indicate up to 50% damage and 50% function impairment. violete would be up to 65% damage, but still 50% function impairment, while red would indicate up to 85% damage with 75% impairment. Flashing red would indicate up to 99% damage and 100% lose of functionality. black means that section/subsystem has been destroyed and must be rebuilt before the functionality can be restored.
example:
   - Phaser array 3 has been destroyed, lowering the ships combat capabilities.
   - deck 6, section 8 has been destroyed. 8 crew members must be housed in other quarters, raising their stress levels by 2 points.

- Voyager crew roster:
	-manage crew roster for a ship.
		-able to assign officers
			-ex: First Officer
		-able to assign personell to different departments
			-ex: assign ensin Peller to medical as medical support.
		-able to recruit new crew members up to max ship capacity
			-Department list:
				- Engineering
					- Chief Engineer
					- transporter chief(s)
					- Crew Chief
			- science
				- Medical
					- Chief medical officer
			- Astro-Metrics 
			- life sciences
			- infectious diseases and mediums
			- genetics
			- Operations
				- Navigation
				- Stellar Cartography 
			- tactical Officer
				- security chief
				- security
		- able to assign personell to mission for X-time or until mission complete
	- character attributes include: 
		-name
		-age
		-grade
		-species
		-rank
		-bio entry
		-mission list
		-mission specialisty
		-special equipment (Used to denote anything removed from human standard, could be species based such as Katarain horns, Klingon 8-chambered heart etc. Would not include things like Ocompa's ears or Talaxian lungs)
		-ranged combat(Attribute used when character is engaged in ranged combat. Value 0-1000)
		-hand to hand combat(Attribute used when character is engaged in hand to hand combat. Value 0-1000)
		-HP (Health)
		-medical status (notes of effects such as limb damage [which effect ranged combat if arm, and hand to hand if leg], illness [such things include contracting the phage])


12-12-2017 (3:38pm):
Discussion with Joel. need to focus on segments for development of concept. So for characters, what are the stats, what do those stats effect, how are those states effected. That sort of thing.

To Do: 
Character class:
Define what each attribute is.
Define what each attribute does.
Define what each attribute effects, if any.
Define how each attribute is affected.
attributes -
	name
	gender 
	rank
	mission role
	science rating
	engineering rating
	ranged combat rating
	hand to hand combat rating
	regeneration
	stress
	fortitutde
	mental fortitude
	morale

other thoughts:
how is combat handled? how would things like phasers vs kazon disruptors effect combat? 
Levels of disabilities:
I want every level of disability from "It's a minor rash" which occasionally causes the crew member to take .1% longer to complete a task, up to "Full life support" making all taskes excruciatingly hard to accomplish (This would be like Pike in a wheel chair) and still have death as a possible result.
Joel: have 5 or six levels of diability ranging from "Fully healed" This ranking would apply to each part of the body.
body parts:
0 - Head
1 - Torso
2 - Right arm
3 - Left Arm
4 - Right leg
5 - Left Leg
6 - legs




0 - "Fully healed"
1 - "minor irratants, scratches, maybe cuts, possibly having eaten Nelix's cooking."
2 - "major irratants, heavy scratches, cat 1-2 burns, not life threatening on their own, painful but only a little affect to performance. Say like a 10% decrease in abilities (would it effect all abilities?)
3 -  "major deterrent from use. 50~75% decrease in abilities
4 - "debilitated and not useful due to injury, but will recover in time" 
5 - "Completely useless due to injury (Example: Nelix loosing his lungs)"

12-14-2017 (3:17pm):
Something I would like to impliment in the program. Each time a 'New Game' is loaded, the player would have the option to "Include characters from the show" or to "Not include characters from the show." 
If they opt to include the characters, then they will presented with a screen to select which characters they can include. Otherwise all the characters are randomly generated for each 'new game'.

12-27-2017 (Vulpus)
Each crew member would have their respective stats including race,(racial buffs/debuff, language barriers?)
- I hadn't originally considered language barriers but being asked the question is making me think about it. At the level the game operates I don't think it would be a benefit to make it speccific languages, but rather a generic communication. So like Torroes would have a moderate 'communication' stat, but Tuvok and Kes would have much higher stats. Tuvok because of his controlled demeanor and rational mind and Kes because of her Telepathy.

gender,(should this really effect stats or just be a boolean for social situations in game)
- Yes there would be gender modifiers but it would be influenced by species. So like human male, vs human female:  1(race) * 1.05(male) bonus to strength versus 1(race) * 1(female) bonus to strength.

if i roster the same male and female long enough will they have a relationship? will there be a sex/love stat?
- there can be friendship/romantic involvement. 
Thoughts on this:
- having someone on the ship/mission that the character is friends with reduces stress levels by a given percentage.
- having some on the mission that the character is in love with would decrease the characters effective thinking (worrying about your love).

can there be children to add to rosters? eugenics, can i breed stats?
- No you can not breed stats. Children is something to consider, but there are two things to consider. 1- With 200 max pop on the ship and needing a bare minimum of 75 to operate the ship (that is operate, not operate it effectively) there won't be a lot of room for 'breeding'. So while children can occure, I don't it to be an event that occures more then 2 to 3 times per calendar year in-game.

human security officer + vulcan security officer = high as fuck hand to hand stats?
- um... not sure what you are asking here. I mean a Vulcan security officer would certainly have higher HtH and Strength Stats then a human one.

rank,(based on merit of decisions made during missions or on exp and general time spent deployed?)
- Rank is something that the character is assigned at generation. However, as the character gains XP it will gain the option to be promoted. 
note: Need to compile list of ranks.

mission role,(can this change during a mission? can they return from a mission "kim demoted because chikote is dead, its kims fault")
- Change in rank will always be as a result of player action. The game will not change rank, but the player always has the option to demote someone, and when the character reaches a level threash hold that character will have the option to be promoted to a given rank.
-The character is not required to be promoted. You can keep Kim an ensign if you like even if he gains sufficient XP to be promoted to commander.
- A character can not skip a rank. They can not go from Leiutenant JG to Lt. Commander for instance. They would need to be promoted to Full Leiutenent, and then to Lt. Commander.

science rating,(improved steady while on ship sporatic during mission? race effect growth rate?)
- Um... not sure what you are asking.

engineering rating,(same question as science rating)
- And just like with science rating, not sure what you are asking.

ranged combat rating,(include primitive weapons? makeshift bow or atlatl while planet side etc etc?)
- Ranged combat is used to determine how effective the character in ranged combat regardless of the weapon in question. However, a phaser rifle is going to cause more damage to a target then a make shift bow.

hand to hand combat rating,(with or without weapons or both same skill?)
- same skill regardless. Weapons can effect the damage inflicted.

regeneration,(race specific? being on ship increases rates? during mission slows?)
- Correct on all accounts. For example: 7 of 9 would have a very high regeneration rate when she is on the ship, while Janeway would have a low-medium regeneration rate when on a mission.
- Regeneration rates can be effects by availible supplies such as food, energy, water, or medical supplies.

stress,(yet again race effected? would this fall under mental fort? too much time on ship without mission cause stress?)
- stress can be effected by race. Klingons for instance would have a negative modifier to handling stress while Vulcans would have a bonus to it. 
- Not sure about the on-ship vs off-ship question. Will need to think on that.

fortitutde,(can this be trained?, race effect?, gender effect?)
- I need to do some brain storming to really figure out what fortitude is. My original thought was about how physically resillient a character is, so like Be'Lanna and 7 of 9 would be really high, but like Kes would be fairly low.

mental fortitude(vulcans get a bonus, race effect again? effected by stress and morale? all three stats seem related)
- Vulcans would definitly get a bonus here, as would Kes. This stat is intended to be used to reference psychic type attacks or conditions. So a higher mental fortitude would indicate the character is less likely to sucumb to possession, telepathic suggestion, etc.

morale.(same questions as stress and mental fort. time on/off ship good or bad effect)
- morale can not be trained, but can be affected by a variety of factors including the characters relationship with others (being with people they like raises morale, being with people they don't like lowers it), stress will lower it, lack of food lowers it, lack of medical supplies will lower it. The big thing is that the morale is a meassure of how readily satisified the character is. If it gets too low (a value that would be assigned on a per-character basis) then there is an increased chance of the character performing poorly at their assignments or even rebelling.


resources effect? does the ship and supplies have stats which could effect the characters?)
- Yes, the supplies on the ship do effect the characters.
- Too little food: negative effect on moral, increasing stress, decreases regeneration rates. Engineering, science, Ranged Combat, and HtH tests would be negatively effected.
- too little energy: negative effect on moral, increasing stress
