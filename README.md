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

- [ ] **Numbers**:

*Les variables peuvent aussi n'être que des valeurs numériques. Un nombre avec une virgule s'appelle un **float**. Il est possible de définir des floats avec des nombres après la virgule (dot) ou simplement en incluant une virgule (dot) à la fin. Il est aussi possible de définir un float avec une signification scientifique, avec un **e** indiquant la puissance 10.*

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

- [ ] **Division**:

*Dans Python 2, il est possible de diviser deux entiers pour obtenir un entier comme résultant. Lorsque le quotient est un nombre entier, cela fonctionne bien.*

```py
quotient = 6/2
# the value of quotient is now 3, which makes sense
```

*Mais si les nombres ne se divisent pas uniformément, le résultat de la division sera alors tronqué en un nombre entier. Le quotient sera donc arrondi à un nombre entier.*

```py
quotient = 7/2
# the value of quotient is 3, even though the result of the division here is 3.5
```

*Pour obtenir un résultat flottant, les développeurs modifient soit le numérateur, soit le dénominateur (ou les deux) pour en faire un flottant.*

```py
quotient1 = 7./2
# the value of quotient1 is 3.5
quotient2 = 7/2.
# the value of quotient2 is 3.5
quotient3 = 7./2.
# the value of quotient3 is 3.5
```

- [ ] **Multi-line Strings**:

*Parfois, il arrive que le string fasse plusieurs lignes lorsque le code est complexe. Pour ce faire, il convient d'insérer **"""***.

```py
address_string = """136 Whowho Rd
Apt 7
Whosville, WZ 44494"""
```

- [ ] **Boleans**:

*Lorsqu'il est nécessaire d'avoir une variable qui est **True** ou **False**: c'est un **Bolean**. Ce type de données ne prendra qu'une des deux données. Avec Python, les boleans sont définis par les mots **True** ou **False**. Un bolean est un cas particulier d'un entier. Une valeur True correspond à une valeur entière de 1 et se comportera de la même manière. La valeur False correspond à une valeur entière de 0.*

```py
a = True
b = False
```

```py
# Hi! I'm Maria and I live in script.py.
# I'm an expert Python coder.
# I'm 21 years old and I plan to program cool stuff forever.
age_is_12 = False
name_is_maria = True
```

- [ ] **ValueEror**:

*Python affecte automatiquement une variable au type de données approprié en fonction de la valeur qui lui est attribuée. Une variable avec la valeur **7** est un **entier**, **7.** est un **flottant** et **"7"** est un **string**. Parfois, il est nécessaire de convertir des variables en différents types de données. Par exemple, si nous souhaitons imprimer un entier en tant que partie d'un string, il faudrait alors convertir cet entier en un string en premier. Pour ce faire, il convient d'utiliser **str()**.*

```py
age = 13
print "I am " + str(age) + " years old!"
# this would print: 
>>> "I am 13 years old!"
```

*Si le string est "7" et qu'il convient d'effectuer des opérations arithmétiques, il convient de convertir en un type de données numériques. Pour ce faire, il convient d'utiliser **int():**.*

```py
number1 = "100"
number2 = "10"

string_addition = number1 + number2 
#string_addition now has a value of "10010"

int_addition = int(number1) + int(number2)
#int_addition has a value of 110
```

*Si **int()** est utilisé sur un nombre à virgule flottante, il arrondira alors le nombre vers le bas. Pour conserver la valeur décimale, il convient d'utiliser **float():**.*

```py
string_num = "7.5"
print int(string_num)
print float(string_num)
>>> 7
>>> 7.5
```

