# Tips
C'est un dépot pour mes tips
## Commandes pour la connexion via SSH

``bash
ssh-keygen -t ed25519 -C "email@mail.com"
``

``bash
ssh -T git@github.com
``

## Code pour la configuration de base d'un fichier vue dans les snippets de vscode

```js
{
// Place your snippets for vue here. Each snippet is defined under a snippet name and has a prefix, body and
// description. The prefix is what is used to trigger the snippet and the body will be expanded and inserted. Possible variables are:
// $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders. Placeholders with the
// same ids are connected.
// Example:
// "Print to console": {
//  "prefix": "log",
//  "body": [
//      "console.log('$1');",
//      "$2"
//  ],
"description": {
    "prefix": "vvue",
    "body": [
      "<script setup>\n\n",
      "</script>\n\n",
      "<template>\n",
      "<div>\n",
      "$1\n",
      "</div>\n",
      "</template>\n\n",
      "<style scoped>\n\n",
      "</style>"
    ],
  }
}
```

## Quelques lignes de commandes django

```bash
python -m venv venv
source venv/Scripts/activate
python -m pip install -r backscript/requirements.txt
py manage.py startapp nom_application(pour créer une application , on met le nom du projet)
python manage.py runserver
```

#### Pour les migrations  :
```bash
py manage.py makemigrations nom_de_l_application
python manage.py migrate --database=nom_de_la_bdd
```
- Installation: py -m pip install django-cors-headers
- ajout de ceci au niveau de INSTALLED_APPS dans le fichier settings.py: 'corsheaders',
- Ajout de ceci au niveau de MIDDLEWARE dans le fichier settings.py: 'corsheaders.middleware.CorsMiddleware',
- Ajout de ceci dans le fichier settings.py: CORS_ALLOWED_ORIGINS = [
    'http://localhost:3000',
]

## Quelques notes JS
````js
JS NOTES

On utilise var, let et const pour déclarer des variables.
Avec let, on ne pourra plus redéclarer la variable mais la réassigner (recommandé). 
Elle est aussi limitée à la portée du bloc.

"=" est l'opérateur d'assignation, il permet d'attriibuer une valeur à une variable.

Incrémentation et décrémentation
++a, a est incrémenté avant son utilisation 
a++, a est utilisé avant son utilisation
Ex:
a = 6;
b = ++a //b=7, a=7
b = a++ //b=6, a=7

On peut convertir des nombres décimaux en entiers en utilisant les fonctions parseInt().
let floatNum = 10.5;
let num = parseInt(floatNum); // Convertit le nombre décimal 10.5 en un nombre entier

On peut aussi convertir des nombres entiers en décimal avec les fonctions parseFloat()

Fonctions mathématiques

Math.sqrt(x) //racine carrée

Math.pow(a,b) ou a ** b//puissance

let nombre = 3.7;
let arrondi1 = Math.round(nombre); // arrondi1 vaut 4
let arrondi2 = Math.floor(nombre); // arrondi2 vaut 3
let arrondi3 = Math.ceil(nombre); // arrondi3 vaut 4

Math.abs(nbr) //valeur absolue

Math.random() //Générer des nombres aléatoires, 0 inclu et 1 exclu.

Pour la concaténation des string, on utilise "+"

La propriété .length est utilisé pour troouver la longueur d'un string

Les tableaux peuvent être créés en utilisant des crochets [] ou le constructeur Array.
````

