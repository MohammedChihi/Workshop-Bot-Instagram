# Workshop Bot Instagram 

WORKSHOP

Pourquoi faire un bot instagram ?
Vous voulez gagnez plus de followers sur votre compte instagram ? Vous en avez marre des technique classique du type follow quelqu'un se faire follow back et ensuite aller vous unfollow ? Vous en avez marre de liker des posts pour que les gens vous follow back ? Les techniques classiques comme les engagements pods vous prennent trop de temps ?

Vous pouvez être streameur, rappeur, youtubeur, etc…, dans toutes ses situations plus de visibilité est égal à plus d'opportunités. Passez des heures par jour à faire des tâches répétitives sur instagram est plutôt énervant, c’est pourquoi il faut penser à une autre stratégie afin de gagner des followers.
 
Bonne nouvelle il y a plusieurs technique, soit vous payez une entreprise qui vous fera monter vos followers (avec des compte insta fake (des bots)) ce qui est souvent mal vu et pas du tout discret parce que passer de 3k followers à 40k en moins de 2 heures n’est pas trop naturel. Sois vous payer un bot instagram qui likera des posts pour vous, ce genre de bots coûte souvent chère, soit vous le faites vous même ce bot.
 
Je tiens a vous rappelez qu’Instagram est de plus en plus strict avec l’automatisation de tâche. Plusieurs personnes ont déjà essayé cette technique et se sont fais ban leurs compte instagram. Ce tuto a pour objectif de vous expliquer le fonctionnement d’un bot instagram.
 
On codera notre bot Instagram en Python, parce que c’est un langage très populaire et facile d’utilisation pour l'écriture de script.
 
Pour info nous allons utiliser un package qui va nous permettre de contourner l’API d’instagram, vu qu’instagram a fortement limité l’utilisation de son API, il n’est plus possible actuellement de créer des bots en faisant des calls au serveurs d’Instagram directement. Donc plutôt que de faire des call a l’API le package que nous allons utilisé va émuler une fenêtre de navigateur et générer des clics aux endroits voulu.
 
 
 
 
 
 
 
Installation:
Pour commencer j’imagine que vous avez tous la librairie python sur vos pc mais au cas ou, voici la commande pour installer python :
sudo yum install python


Pour info il y a plusieurs librairie qui permettent de coder des bot instagram mais la librairie la plus utilisé est InstaPy, qui est une librairie open source la plus développée et qui utilise Selenium. Selenium est le langage mère qui a permit à Tim Grossmann de créer sa propre librairie InstaPy.

Pour installer InstaPy : 
pip install instapy

https://github.com/InstaPy/InstaPy


JE TIENS A VOUS RAPPELEZ DE NE PAS FAIRE CE WORKSHOP AVEC VOTRE COMPTE INSTA PRIVEE VEILLEZ À BIEN CREER UNE NOUVELLE ADRESSE MAIL ET UN NOUVEAU COMPTE INSTA AYANT AUCUN LIEN AVEC LE COMPTE INSTAGRAM QUE VOUS UTILISEZ D’HABITUDE !!




Ex01:
Créez un fichier en .py et commencez par simplement créer votre session avec votre mot de passe, nom d’utilisateur.


Ex02:
Maintenant lancez votre session avec tous les paramètres que vous voulez (comme le type de profil que vous voulez suivre, s’ils ont beaucoup d’abonnés, s'ils sont eux même follow a beaucoup de monde ou pas, etc...). Il y a une infinité de paramètres à ajouter, n'hésitez pas à vous faire plaisir ou à faire en fonction de vos besoins.








Ex03:
Quand les influenceurs publient des photos insta, ils mettent tout le temps des Hashtag, ces derniers permettent à la photo d'être mieux référencé et donc d'être affiché sur le feed des personnes qui seront intéressé par ce genre de photo.
Disons que vous êtes quelqu’un qui aime la cuisine, du coup qui fait beaucoup de recherche par rapport à la cuisine, alors soyez beaucoup plus apte a avoir sur votre feed des photo ou vidéo de cuisine.


Je vous propose maintenant de faire en sorte que votre compte ne follow pas les personnes ayant posté des photos sur le foot. Vous allez devoir ajouter quelques lignes permettant d'éviter de suivre  les comptes avec des photos de foot.

Ex04:
Afin de gagner des followers, va falloir commencer par faire en sorte que votre bot follow lui-même des comptes qui ont les mêmes centres d'intérêt que vous afin que ces derniers vous follow back et que vous puissiez augmenter votre fan base.

Essayez de mettre en place un pourcentage de compte a follow pour pas que votre bot follow tous les comptes qu’ils sélectionnent.

Ex05:
Toujours dans le même objectif d’augmenter votre fanbase, vous allez essayer de liker des images contenant des hashtag qui vous intéresse, disons que votre page est accès sur la cuisine, vous allez donc demander à votre bot de liker toutes les images avec le hashtag cuisine.

Ex06:
Afin de rendre votre bot le plus réaliste possible, vous allez lui demander de commenter les posts qu'il like. De préférence votre bot ne doit pas commenter tout les post avec les mêmes commentaires, du coup vous allez lui proposer une liste de commentaire à mettre sous les posts et il s’occupera d’une maniere aleatoire de mettre des commentaire ou non, en fonction d’un pourcentage que vous lui imposerez. Disons que votre bot mettra un commentaire sur 60% des post qu’il like.

Ex07:
Afin d’optimiser votre compte, vous allez devoir vous désabonner aux comptes qui ne vous ont pas follow back. De plus essayer de vous désabonner de manière intelligente, c'est-à-dire, les comptes les plus anciens qui vous ne follow pas, vous pouvez ajouter un temps maximum de temps que les compte ne vous ont plus follow. 
De plus je vous conseille d’ajouter un délai après chaque désabonnement afin de ne pas trop spammer Instagram.
Ex08:
Il ne vous reste plus qu’à rejoindre des pod Instagram, afin d’avoir plus de visibilité, ajouter le fait de ne pas ajouter de commentaire.


Ex Bonus:
Essayez d’ajouter plein de fonctionnalités à votre bot, essayez de le perfectionner au maximum. Faites vous plaisir, est ce que votre objectif est d’avoir le plus de followers le plus rapidement possible, ou vous êtes plus dans la sélection de votre communauté ? 
Personnalisez le au maximum !!


Comment faire fonctionner le bot python ?
Il y a plusieurs manières de lancer et héberger votre bot Instagram, vous pouvez soit le lancer sur un environnement virtuel, soit le lancer sur un raspberry pi, soit sur une image docker, soit dans le cloud grâce à digitalocean.

La création d’un environnement virtuel est la technique la plus simple pour exécuter votre bot. C’est pour cela que je vais vous présenter cette technique, de plus toutes les autres techniques sont payantes, soit il nous manquera le matériel nécessaire.

ENVIRONNEMENT VIRTUEL :

Exécutez les commandes suivante afin de mettre en place votre environnement virtuel :

``` python3 -m venv “mettez le nom que vous voulez” ```

ensuite vous exécutez votre code dans votre environnement.
