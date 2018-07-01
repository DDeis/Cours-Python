# Cours - Python
## String and console output

- [ ] **Strings**:

*Un autre type de données utiles est la châine (**string**). Une string peut contenir des lettres, des chiffres et des symboles. Les chaînes doivent être contenues dans des **""**.*

```py
#Dans l'exemple, nous créons un nom de variable définit à la valeur de la chaîne "Ryan". Nous mettons également l'âge à "19" et la nourriture à "fromage".

name = "Ryan"
age = "19"
food = "cheese"
```

- [ ] **Escaping characters**:

Certains caractères peuvent poser problème. Pour ce faire, il convient d'utiliser: \ 

```py
'There's a snake in my boot!'
```

```py
#Ce code n'est pas bon puisque Python pense que l'apostrophe dans "There's" marque la fin d'une string. Donc il convient d'écrire: 
```
```py
'There\'s a snake in my boot!'
```

- [ ] **Acces by index**:

*Chaque caractère dans une string peut être assigné à un nombre. Ce nombre is appelé **index**.*

```py
c = "cats"[0]
n = "Ryan"[3]
```
```py
#Dans cet exemple, une variable a été crééee appelée "c" et lui a été assigné le caractère à l'index "0" de la string "cats". Puis, une nouvelle variable "n" avec le caractère à l'index "3" de la string "Ryan". 
```

- [ ] **String methods**:

*Les String methods permettent d'effectuer des tâches spécifiques pour les châines.*

```py
len()
lower()
upper()
str()
```

*len() permet d'obtenir la longueur (le nombre de caractères) de la string.*

```py
parrot = "Norwegian Blue"
print len(parrot)
>>> 14
```
```py
#Sur la ligne 1, nous avons crée une variable nommée "Norwegian Blue". Sur la ligne 2, nous avons demandé de calculer le len() de la variable "parrot". Ce qui permet d'afficher le nombre de caractères contenus dans la variable "Noregian Blue" qui est 14.
```

*lower() permet de se débarrasser de toutes les majuscules contenues dans la string. Il convient de l'écrire comme cela:*

```py
"Ryan".lower()
```
```py
parrot = "Norwegian Blue"
print parrot.lower()
>>> norwegian blue
```

*upper() permet de créer la string complètement en majuscule.
```py
parrot = "Norwegian Blue"
print parrot.upper()
>>> NORWEGIAN BLUE
```

*str() transforme les non-strings en strings.*
```py
str(2)
```
```py
#Declare and assign your variable on line 4 then call your method on line 5.
```
```py
pi = 3.14
print str(pi)
>>> 3.14
```

- [ ] **Print variables**:

```py
"""Assign the string "Ping!" to
the variable the_machine_goes on
line 5, then print it out on line 6!"""

the_machine_goes = "Ping!"

print the_machine_goes
>>> Ping!
```

- [ ] **String Concatenation**:

*L'opérateur **+** entre les strings permet de les ajouter les unes après les autres. Il y a des espaces à l'intérieur des guillemets et après l'opérateur. C'est la concatenation.*
```py
#Print the concatenated strings "Spam", "and", "eggs".
```
```py
print "Spam " + "and " + "eggs"
>>> Spam and eggs
```

- [ ] **Explicit string conversion**:

*Parfois, il est nécessaire de combiner une string avec quelque chose qui n'est pas une string. Pour ce faire, il convient de convertir la non-string en string.*
```py
print "I have " + str(2) + " coconuts!"
```
*Cela imprimera "I have 2 coconuts!". La méthode str() convertit les non-strings en strings. Dans l'exemple ci-dessus, on convertit le nombre 2 en une string puis on concaténise les strings ensemble.*
```py
print "The value of pi is around " + str(3.14)
>>>The value of pi is around 3.14
```

- [ ] **String formatting with %**:

*Pour imprimer une variable avec une string, il existe une meilleure méthode que la concaténation des strings ensemble. L'opérateur **%** après la string est utilisé pour combiner une string avec des variables. L'opérateur **%** remplacera le **%** de la string par la variable de la string qui le suit.*
```py
name = "Mike"
print "Hello %s" % (name)
```
*Pour imprimer une variable qui est un nombre entier, il convient d'ajouter des zéros en utilisant **%02d**. Le **0** signifie "pad avec zéros", le **2** signifie "pad à 2 caractères" et le **d** signifie que le nombre est un entier signé (positif ou négatif).*
```py
day = 6
print "03 - %s - 2019" %  (day)
# 03 - 6 - 2019
print "03 - %02d - 2019" % (day)
# 03 - 06 - 2019
```
```py
print "The %s who %s %s!" % ("Knights", "say", "Ni")
# This will print "The Knights who say Ni!"
```



