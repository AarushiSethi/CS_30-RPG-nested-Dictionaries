# CS_30-RPG-nested-Dictionaries

#2D Arrays and nested dictionaries_Aarushi Sethi
#CS 30: RPG Nested Dictionaries
#Date: 29/4/22
#Adding properties to your characters, locations and inventory using nested dictionaries


#inventories
staff={'Arjun':{'main_role':'Saves many lives','super_power':'Knows the Hotel','health_points':50}
       ,'Headchef':{'main_role':'Keeps people safe','super_power':'knows people','health_points':40},
       'Tanmay':{'main_role':'Takes up duties','super_power':'is obedient','health_points':20}}  #inventory1

police_officers={
    'local police':{'description':'serves the city','damage':15,'protection':30},
    'special squad commander':{'description':'Commands the soldiers','damage':15,'protection':20},
    'special squad soldier':{'description':'Ultimate protection','damage':25,'protection':50}} #inventory2

location={'lounge':'is the safest place in the hotel','hallway':'is the most dangerous place',
          'guest rooms':'are more that 500 in number','service stairs':'are for staff only',
          'terrace':'is beautiful'} #inventory3

#character and traits in Staff
print('character and traits in Staff')

for char, role in staff.items():
    print(f'''{char}\'s main role is that he {role["main_role"]}
{char}\'s super power is that he {role["super_power"]}
{char}\'s health points are {role["health_points"]}\n''')
    
#locations and description
print('locations and description')

for loc in location.keys():
    print(f'{loc} {location[loc]}')
    
#inventories and characteristics
print('\nPolice Officers\n')

for cops, cop in police_officers.items():
    print(f'{cops}:\n Description:{cop["description"]}\n Damage:{cop["damage"]}\n Protection:{cop["protection"]}\n')

