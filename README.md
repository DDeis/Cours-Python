# Cours-Python
## Les bases
- Faire parler Python 2: 
```py
print "Hello, world!"
```
- Faire parler Python 3: 
```py 
print ("Hello, world!")
```
- [ ] **String**: 

*Chaîne de caractères (lettres, nombres, symboles)*
- *Pour combiner des châines de caractères (`string`), utiliser l'opérateur (operator) `+`*
```py
print "Hello" + "world!"
```
- [ ] **Variable**: 

*Donner un nom à une valeur*
```py
say = "Hello, aujourd'hui nous sommes le"
day = "samedi"
todays_date = "30 juin 2018"
print say + day + todays_date
```
- [ ] **Arithmetic**:
```py
addition = 12381 + 2 
substraction = 981 - 312
multiplication = 38 * 982
division = 540 / 45
combinations = 129 + 1345 + 120 / 6 - 12 
```
- **Modulo operator**: 
Permet de calculer le reste (**remainder**) d'une opération
```py
is_this_number_odd = 15 % 2
is_this_number_divisible_by_seven = 133 % 7
```

- **Exemples**: 

*In the above example, we use the price of a sandwich to calculate sales taxe. After calculing the tax we add it to the total price of the sandwich. Finally, we complete the transaction by reducing our money_in_wallet by the cost of the sandwich (with tax).*

```py
money_in_wallet = 40
sandwich_price = 7.50
sales_tax = .08 *
sandwich_price += sales_tax
money_in_wallet -=
sandwich_price
```

*We're trying to figure out how much it rained in the past year.*

```py
january_to_june_rainfall = 1.93 + 0.71 + 3.53 + 3.41 + 3.69 + 4.50
annual_rainfall = january_to_june_rainfall

july_rainfall = 1.05
annual_rainfall += july_rainfall

august_rainfall = 4.91
annual_rainfall += august_rainfall

september_rainfall = 5.16
annual_rainfall += september_rainfall

october_rainfall = 7.20
annual_rainfall += october_rainfall

november_rainfall = 5.06
annual_rainfall += november_rainfall

december_rainfall = 4.06
annual_rainfall += december_rainfall
print annual_rainfall
```

- [ ] **Comments**:

*Permet d'insérer des commentaires pour simplifier la compréhension du code. Pour ce faire, il convient d'insérer le symbole **#**

```py
#this variable counts how many rows of the spreadsheet we have:
row_count = 13
```

    [ ] **Numbers**:

*Les variables peuvent aussi n'être que des valeurs numériques. Un nombre avec une virgule s'appelle un **float**. Il est possible de définir des floats avec des nombres après la virgule (dot)ou simplement en incluant une virgule (dot) à la fin. Il est aussi possible de définir un float avec une signification scientifique, avec un **e** indiquant la puissance 10.*

```py
int1 = 1
int2 = 10
int3 = -5
float1 = 1.0
float2 = 10.
float3 = -5.5 
#this evaluates to 150: 
float4 = 1.5e2
```

- 