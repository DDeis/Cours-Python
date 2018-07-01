# Cours - Python
## Conditionals and control flow

- [ ] **Définition du Flow**:

*Jusqu'à présent, les programmes Python qui ont été écrits ont eu un esprit unique: ils peuvent ajouter deux nombres ou imprimer quelque chose, mais ils n'ont pas la possibilité de choisir l'un de ces résultats par rapport à l'autre.* 

*Le **flow** (flux de contrôle) donne cette possibilité de choisir parmi les résultats en fonction de ce qui se passe d'autre dans le programme.*

*Les comparators vérifient donc si une valeur est (ou n'est pas) égale à, supérieur à (ou égale à), ou inférieur (ou égale à) une autre valeur.*

*Il convient de noter que **==** compare si deux choses sont égales alors que **=** assigne une valeur à une variable.*

*Les comparators résultent de **True** ou **False** qui sont des **boleans**.*


- [ ] **Les comparators**: 

**Equal to (==)**
```py
>>> 2 == 2
True
>>> 2 == 5
False
```
**Not equal to (!=)**
```py
>>> 2 != 5
True
>>> 2 != 2
False
```
**Less than (<)**
```py
>>> 2 < 5
True
>>> 5 < 2
False
```
**Less than or equal to (<=)**
```py
>>> 2 <= 2
True
>>> 5 <= 2
False
```
**Greater than (>)**
```py
>>> 5 > 2
True
>>> 2 > 5
False
```
**Greater than or equal to (>=)**
```py
>>> 5 >= 5
True
>>> 2 >= 5
False
```

- [ ] **To Be and/or Not to Be**:

*Les boolean operators comparent les instructions et produisent les valeurs booléennes. Il y a trois opérateurs: **and, or et not**.*

**And**: vérifie si les deux déclarations sont vraies. 

A | B | A AND B
-- | -- | --
True | True | True
True | False | False
False | True | False
False | False | False

```py
1 < 2 and 2 < 3 = True
>>> True and True = True
```

**Or**: vérifie si au moins une des conditions est vraie. 

A | B | A OR B
-- | -- | --
True | True | True
True | False | True
False | True | True
False | False | False

```py
1 < 2 or 2 > 3 = True 
>>> True or False = True
1 > 2 or 2 > 3 = False 
>>> False or False = False 
```

**Not**: donne le contraire de la déclaration. 

A | NOT A
-- | -- 
True | False
False | True
```py
not 10 % 3 <= 10 % 2 = True 
```

- [ ] **This and That (or This, But, Not That!)**:

*Les boolean operators ne sont pas simplement évalués de gauche à droite. Tout comme avec les opérateurs artihmétiques, il existe un ordre des opérations pour les opérateurs booléens.*

**And** * n'est pas évalué en premier et est évalué ensuite.*

**Not** *est évalué en premier*

**Or** *est évalué en dernier. Par exemple "True or not False and False" renvoie à "True".*

**L'ordre est donc: not, and, or**

*Les parenthèses () s'assurent que les expressions sont évaluées dans l'ordre souhaité. Tout ce qui est entre () est évalué comme sa propre unité.*

```py
False or not True and True = False

False and not True or True = True

True and not (False or False) = True

not not True or False and not True = True

False or not (True and True) = False
```

- [ ] **Conditional statement syntax: IF**:

***If** est une instruction conditionnelle qui exécute du code spécifié après avoir vérifié si son expression est **True**.*
```py
if 8 < 9:
  print "Eight is less than nine!"
  ```

  *Dans cet exemple, 8<9 est l'expression cochée et l'impression "Eight is less than nine!" est le code spécifié.*

  *Attention à l'indentation avant la déclaration d'impression. Cet espace, appelé **white space** est la façon dont Python sait que nous entrons un nouveau bloc de code. Python accepte de nombreux types d'indentation pour indiquer les blocs. Ici, quatre espaces sont utilisés mais ailleurs, il est possible de rencontrer des indetations ou des tabulations à deux espaces (que Python verra comme différents des espaces).*

  *Si l'indentation d'une ligne à la suivante est différente et qu'il n'y a pas de commande (comme **if**) indiquant un bloc entrant, alors Python déclenchera une **IndentationError**. Ces erreurs pourraient signifier, par exemple, qu'une ligne avait deux espaces mais que la suivante en avait trois. Python essaie d'indiquer où cette erreur s'est produite en imprimant la ligne de code qu'il n'a pas pu analyser et en utilisant ^ pour pointer vers où l'indentation était différente de ce qu'il attendait.*

- [ ] **Conditional statement syntax: ELSE**:

*L'instruction **else** complète l'instruction **if**. Une paire **if/else** dit "si cette expression est vraie, exécuter ce bloc de code en retrait; sinon, exécuter ce code après l'instruction else"*.
```py
if 8 > 9:
  print "I don't printed!"
else:
  print "I get printed!"
  ```

  - [ ] **Conditional statement syntax: ELIF**:

****Elif** est l'abréviation de "else if". Cela signifie "sinon, si l'expression suivante est vraie, faites ceci!". Dans l'exemple, l'instruction **elif** n'est vérifiée que si l'instruction if d'origine est False.*
```py
if 8 > 9:
  print "I don't get printed!"
elif 8 < 9:
  print "I get printed!"
else:
  print "I also don't get printed!"
  ```
