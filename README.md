# STV-The-Long-Journey
Overview of the Project:
This is a fan project to develop a roster management game based on the show Star Trek Voyager. This is not intended to be sold and should not be considered to be sold in any fashion. My primary goal in making this is to under take a project to expand my skills as a programmer, expand my expierence with python speccifically, and to learn how to use Github. 

What is a roster Management game?
Just like the name implies, instead of controlling speccific assets you manage those assets by roster. In the case of the plans for this game, the assets to be managed are the crew of the USS Voyager and you manage them by assigning them to missions and departments. So you can assign Ensign Kim to operations, or you can assign him to Sick bay. He will perform better in some departments then others based on his individual traits and skills so you will want to maximize his contributions to the ship by assigning him to departments and missions that suite his skills. However, there could be times where he is the best option for a department or mission that he is only moderatly skilled in due to mission demands or injuried/killed crew members. 


Development notes: This section will be any accumulated notes regarding the game.
==================================================================================================================================
STar Trek Voyager The Long Journey: You would take on the role of Captain Janeway as she attempts to lead the USS Voyager home from the delta quadrant, a journy they by all estimates will take over 75 years. You must pick the right people for the right jobs to maximize your chances not only of survival, but also in gathering supplies to maintain your ship and crew, but also in obtaining additional tech to aide you in your journey. The game itself would would be a roster management game with minimal graphics. The over all idea is you would have a roster of crew members. Each crew member would have their respective stats including race, gender, rank, mission role, science rating, engineering rating, ranged combat rating, hand to hand combat rating, regeneration, stress, fortitutde, mental fortitude and morale. These stats would be used in under taking various missions and assignments. 

So you would have several screens that would allow you to view damage to the ship, details about upgrades to the ship, view crew roster, department assignments, and missions assignments. 

list of screens accessible to the player:
Captains Command center: the CCC provides the overall view of the ship status and crew status. Displaying over all crew morale status.
- crew roster: A complete listing of the ships crew, can be sorted alphabetically, by species, by department, or by rank. Would be able to assign crew member to department from this screen. The department that the crew member is assigned to will be their default posting after they return from an away mission or after medical treatment.
- crew member profile: A detailed view of an individual crew member including their stats, and assembled baground/bio.
- department reports: detailed view of status of the ship by department. Would include information regarding department efficency and status as well as any notes regarding supply short falls and their effects. Would also be able to pull up a list of crew members assigned to this department.
- away team report: Display the current status of any currently active away missions.
- tactical display: would display current status of the ship and it's weapon system. Display would include a wire frame display of the ship with sections picked out in color to denote damage levels. Green would indicate normal operation and no damage. teal would indicate up to 15% damage to that area, but otherwise operational. blue would indicate damge more then 15% and up to 35% with up to 25% impaired functionality. Blue would indicate up to 50% damage and 50% function impairment. violete would be up to 65% damage, but still 50% function impairment, while red would indicate up to 85% damage with 75% impairment. Flashing red would indicate up to 99% damage and 100% lose of functionality. black means that section/subsystem has been destroyed and must be rebuilt before the functionality can be restored.
example:
   Phaser array 3 has been destroyed, lowering the ships combat capabilities.
   deck 6, section 8 has been destroyed. 8 crew members must be housed in other quarters, raising their stress levels by 2 points.

Voyager crew roster:
	manage crew roster for a ship.
	able to assign officers
		ex: First Officer
	able to assign personell to different departments
		ex: assign ensin Peller to medical as medical support.
	able to recruit new crew members up to max ship capacity
		Department list:
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
	able to assign personell to mission for X-time or until mission complete
	character attributes include: 
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
==================================================================================================================================

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
I want every level of disability from "It's a minor rash" which occasionally causes the crew member to take .1% longer to complete a task, up to "Full life support" making all taskes excruciatingly hard to accomplish (This Pike in a wheel chair) and still have death as a possible result.
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
