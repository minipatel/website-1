title=console sous stéroide
date=2018-09-15
type=post
tags=console, outils, cat, ping, man, du, jq, fzf, top, htop, ncdu
status=published-date
~~~~~~

Ci dessous un résumé de l'article que vous retrouverez [ici](https://remysharp.com/2018/08/23/cli-improved) qui recence des outils pour la console qui remplacent avantageusement leurs illustres prédecesseurs. Le tout testé sur OSX.

## bat - (cat)
pour remplacer ```cat``` bienvenue à ```bat```
![Bat screenshot](./bat.png)
* [site officiel](https://github.com/sharkdp/bat)

### Installation de bat
```# brew install bat```

### Les plus 
* coloration syntaxique
* recherche dans le texte
* numérotation des lignes

## prettyping - (ping)
pour remplacer ```ping``` bienvenue à ```prettyping```
![PrettyPing screenshot](./prettyping.png)
* [site officiel](http://denilson.sa.nom.br/prettyping/)

### Installation
```# brew install prettyping```

### Les plus 
* évolution graphique des temps de réponses

## fzf (ctrl-r)
Un couteau suisse de recherche dans les fichiers votre historique ... etc.
![fzf screenshot](./fzf.png)
* [site officiel](https://github.com/junegunn/fzf)

### Installation de  fzf
```# brew install fzf```

### Usage
rechercher dans votre historique avec classe (CTRL-R)
rechercher dans vos fichiers avec preview ```fzf --preview 'bat --color always {}'```

### Les plus 
* Ah bon on pouvez faire tout cela.

## bashhub (history)
votre historique dans le cloud.
![bashhub screenshot](./bashhub.png)
[site officiel](https://bashhub.com/)

### Installation de  bashhub
zsh ```# curl -OL https://bashhub.com/setup && zsh setup ```
bash ```# curl -OL https://bashhub.com/setup && bash setup ```

### Usage
CTRL-b
bh -i 

### Les plus 
* Ah bon on pouvez faire tout cela..

## htop (top)
Suivre vos performance système.
![htop screenshot](./htop.png)
* [site officiel](http://hisham.hm/htop/)

### Installation
```# brew install htop```

## diff-so-fancy (diff)
![diffsofancy screenshot](./diffsofancy.png)
* [site officiel](https://github.com/so-fancy/diff-so-fancy)

### Installation
```# brew install diff-so-fancy```

## fd (find)
rechercher dans vos dossier
![fd screenshot](./fd.png)
* [site officiel](https://github.com/sharkdp/fd/)

### Installation
```# brew install fd```

## ncdu (du)
Interactive disque usage.
![ncdu screenshot](./ncdu.png)
* [site officiel](https://dev.yorhel.nl/ncdu)

### Installation
```# brew install ncdu```

### Usage
* ```ncdu --color dark```

## jq (interpreter les flux json)
Interpreter les flux json comme un boss
![jq screenshot](./jq.png)
* [site officiel](https://stedolan.github.io/jq/)

### exemple 
``` bash
 # curl 'https://api.github.com/repos/tisseurdetoile/website/commits?per_page=5' | jq '.[0] | {message: .commit.message, name: .commit.committer.name}'
 
 {
   "message": "ajout d'un post de blog",
   "name": "TisseurDeToile"
 }
```
### Installation
```brew install jq```
