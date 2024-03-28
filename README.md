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
conj = [verbe[:-2]+"e", verbe[:-2]+"es", verbe[:-2]+"e", verbe[:-2]+"ons", verbe[:-2]+"ez", verbe[:-2]+"ent"]
conjug = [obj for pair in zip(pron,conj) for obj in pair]
separator = " "
conjugation = separator.join(conjug)
print('La conjugaison de "'+verbe+'" au présent de l\'indicatif :',conjugation )
#Compléter ci-dessous
