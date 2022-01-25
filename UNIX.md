# UNIX

[about](https://swcarpentry.github.io/shell-novice/)

## Se familiariser avec le shell unix

commande, options (commence avec "-") et arguments 

linux is case-sensitive

```bash
~ #tilde = plus haut niveau de la machine
ls /#iste le contenu du répertoire courant
la #liste all contents
--help 
man [command] #manuel. q to quit
ls -F #liste détaillée*
ls -l #liste longue: permisssion, user, date de création, dimension du fichier
cd #change directory
clear #clear terminal
pwd #print working directory = path where i am
ls -t #order by most recent, -lt to have a list ordered by date
cd [folder] #change directory
```

syntaxe: 

- répertoires (répertoire = suivi d'un dash folder/) = bleu  
- fichiers = blanc
- something@ = lien symbolique
- something* = fichier exécutable

## Comment naviguer les fichiers et répertoires

```bash
cp #copy [filename*][can me moren ames] [destination]
cp -r #recursive for directories
mv #move
mkdir #Make directory
mkdir -p [smthg/smthg] #make directory and subdirectory
ls -R #list recursive, folders and contents
nano [filenam] #ouvre un fichier
touch [filename] #le crée
mv #move, can also rename 
rm #remove file
rm -r #remove directory / all contents
rm -i #remove interactive to confirm
* #caractère générique, all
ctrl+c #sort de la commande en cours
echo #print in terminal
```



## Pipes et filtres

pipe (tuyeau) : take result from command1 and use it for command2

use |

```bash
wc [filename] # word count. Returns lines, words, chars, filename
wc *.txt #returs list + total
wc -l #nb de lignes
> #redirection, exemple prend le résultat et le met dans un nouveau fichier
>> #ajoute au fichier en question (au lieu de réécrire si le fichier existe déjà)
cat [filenmae] #liste le contenu du fichier dans le terminal
less [filename] #liste les dernières lignes d'un fichier
head [filnemame] #liste les premières lignes. -n [nb lignes à voir]
tail [filename] # liste les dernières lignes d'un fichier.
sort #--help for options. -n : tri numérique (et non alphanumérique pas défaut). -r; reverse sort
wc -l *.txt | sort -n | head -n 1 #counter les lignes des fichers .txt, trier numériquement et afficher la première ligne = le fichier avec le nombre de lignes le plus court
cat file.txt | head -n 5 | tail -n 3 | sort -r > final.txt
cut #sépare en colonnes, avec char séparateur, par défaut [ŧab]. -d : delimiteur. -f: list of fields
cut -d , -f file.txt | sort | uniq #unique results
uniq -c #number -c occurences
```



## Boucles

```bash
for thing in thing_list
do stuff
done

while
{01..09} # séquence
```

## Script

extension .sh pour distinguer d'un txt et montrer que c'est un script

```bash
bash script.sh
```

