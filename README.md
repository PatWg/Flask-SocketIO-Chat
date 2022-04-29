Flask-SocketIO-Chat
===================

# Introduction et crédits
Un exemple de chat en ligne utilisant
[Flask-SocketIO](https://github.com/miguelgrinberg/Flask-SocketIO-Chat). 

Ce répertoire a été quelque peu modifié pour pouvoir être utilisé comme
démonstration dans le cours GymInf sur les réseaux, les adresses IP, et le Web. 

# installation et démarrage
Pour installer ce répertoire, vous pouvez ouvrir votre terminal et cloner ce
répertoire dans le dossier de votre choix:

``` sh
git clone https://github.com/PatWg/Flask-SocketIO-Chat
```

Puis, il est recommandé de créer un environnement virtuel pour en pas impacter
votre distribution Python globale. Un environnement virtuel est comme une
distribution minimal de Python, cloisonnée dans le répertoire où vous l'avez
créé. Pour cela, rendez-vous dans le répertoire qui vient d'être créé suite à la
commande `git` précédente, puis:

``` sh
# On crée l'environnement virtuel dans le répertoire .venv/
python3 -m venv .venv

# On active cet environnement virtuel
source .venv/bin/activate
```

Maintenant que cet environnement est créé et activé, nous pouvons télécharger
les modules nécessaires.

``` sh
pip3 install -r requirements.txt
```

Et enfin, nous pouvons lancer l'application Flask:

``` sh
# Si nous souhaitons juste la lancer en local (i.e., uniquement accessible 
# depuis l'ordinateur ou se trouve le serveur et invisible pour les autres 
# machines sur le même réseau):
flask run


# Si nous souhaitons rendre l'application visible pour les autres machines sur 
#le même réseau (remplacer XXX.XXX.XXX.XXX par votre adresse IP sur le réseau
#auquel vous serez connecté le jour de l'activité):
flask run --host XXX.XXX.XXX.XXX
```

Puis, pour se rendre sur ce chat, il suffit de lancer son navigateur préféré,
puis de saisir dans la barre d'adresse: `XXX.XXX.XXX.XXX:5000/`.
