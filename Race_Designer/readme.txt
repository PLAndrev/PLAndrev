THis part is resposible for race design 
(included predefined)

RACE penalty = PRT + LRT + ENV + IND + TCH

-----------------

PRT penalty: from file

------------------

LRT penalty: from file
calc positives: 0,0,1,2,-18,-54, -43-(6.5 * (NEG -6))
NEG = each level calculated separatlly

calc negatives: 0,0,-1,-1,-14, -30 - (6 * (POS -5))

------------------

[leght bar]
calc bar lenght points (for 70 result is 0)
if center of bar <> 50:
(1) 1.4 * (to 50)
(2) 1.4 * (to 50) -0.25 * (to 75) * (to 75)

[lenght bar penalty]
bars are multiplied by penalties:
for bar 2:
for bar 3:

[growth]
growth = growth value + bar multiplier

[immune level]
give another value of general growth value and bar multipliers

[summarry]
value = growth(immune) + bar * multiplier(growth(immune))
------------------

IND penalty: from tables (sum all values)

------------------

TCH penalty

calc positives + negatives:
difference: from table
plus penalty as "start at tech 3 for all techs exp" if checked;


to do:
LOAD race from file
SAVE race to file
