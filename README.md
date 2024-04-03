# exos
Random exercices

# 1) Écrivez un programme qui demande à l'utilisateur l'infinitif d'un verbe simple du premier groupe, comme par exemple "chanter", puis affiche la conjugaison du verbe au présent de l'indicatif, de la manière suivante :
```
#Entrez l'infinitif d'un verbe du premier groupe : 
#chanter
#La conjugaison de "chanter" au present de l'indicatif :
  #je chante
  #tu chantes
  il/elle/on chante
  nous chantons
  vous chantez
  ils/elles chantent

verbe = input("Entrez l'infinitif d'un verbe du premier groupe : ")
#Compléter ci-dessous
pron = ["je", "tu", "il/elle/on", "nous", "vous", "ils/elles"]
conj = [verbe[:-2]+"e\n", verbe[:-2]+"es\n", verbe[:-2]+"e\n", verbe[:-2]+"ons\n", verbe[:-2]+"ez\n", verbe[:-2]+"ent\n"]
conjug = [obj for pair in zip(pron,conj) for obj in pair]
separator = " "
conjugation = separator.join(conjug)
print('La conjugaison de "'+verbe+'" au présent de l\'indicatif :\n',conjugation )
#Compléter ci-dessous
