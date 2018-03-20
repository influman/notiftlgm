# Installation
Gestion des Notifications via IFTTT pour Telegram, Twitter, Notifications, etc.
    
### Prérequis en fonction de la notification souhaitée
  
Récupérer le code Key du service Webhooks de IFTTT.  
Dans IFTTT.com, après avoir créé un compte le cas échéant, recherchez (rubrique Search) le service Webhooks, et récupérez votre code personnel KEY dans la rubrique Documentation.  
  
 ![WH](https://i.imgur.com/AsmQ2yR.png) 
  
Pour Telegram,  
  
  * Installez sur votre smartphone l'application Telegram, et éventuellement l'application IFTTT (plus simple cependant de gérer IFTTT.com depuis un écran laptop)
  * Dans IFTTT, cherchez cette fois le service Telegram et appareillez le avec IFTTT. La procédure a pour finalité de créer le Bot IFTTT sous Telegram.
  
 ![TLGM1](https://i.imgur.com/rTcoPX8.jpg) 

  * Retour dans IFTTT.com, créez un nouvel Applet dans la rubrique My Applets (Bouton NEW APPLET)
  * Pour la partie +THIS, cherchez Webhooks, sélectionnez "Receive a Web Request", et nommez le déclencheur (Trigger) par exemple "Telegram_eedomus"
   
 ![WH2](https://i.imgur.com/Vjlfr91.png) 
  
  * Pour la partie +THAT, cherchez Telegram, sélectionnez "Send Message", et modifiez Message Text en alignant les trois ingrédients sans espace : Value1 Value2 Value3
  * Sauvegarder votre Applet IFTTT
 
 ![WH3](https://i.imgur.com/qUKzL96.png)  
  
  
Pour Twitter,  
  
Dans IFTTT, cherchez le service Twitter et appareillez le avec IFTTT, deux possibilités :   
- Soit vous avez préalablement créé un compte Twitter privé complémentaire dédié aux tweets de votre maison, et auquel vous abonnerez votre compte Twitter normal.
- Soit vous utilisez votre compte Twitter actuel et vous souhaiter un recevoir un message direct privé (DM).  
  
  * Créez un nouvel Applet dans la rubrique My Applets (Bouton NEW APPLET)
  * Pour la partie +THIS, cherchez Webhooks, sélectionnez "Receive a Web Request", et nommez le déclencheur (Trigger) par exemple "Twitter_eedomus"
  * Pour la partie +THAT, cherchez Twitter, sélectionnez "Post a tweet" dans le 1er cas, ou "Send a direct message to yourself" dans le 2nd
  * Modifiez le message en spécifiant uniquement les trois ingrédients sans espace : Value1 Value2 Value3
  * Sauvegarder votre Applet IFTTT
  
Pour Notifications IFTTT,
  
Ce service IFTTT réalise un push notification direct (iOS ou Android).   
Il vous faut seulement installer l'application IFTTT sur votre smartphone.  
  
  * Créez un nouvel Applet dans la rubrique My Applets (Bouton NEW APPLET)
  * Pour la partie +THIS, cherchez Webhooks, sélectionnez "Receive a Web Request", et nommez le déclencheur (Trigger) par exemple "IFTTT_eedomus"
  * Pour la partie +THAT, cherchez Notifications, sélectionnez "Send a notification from the IFTTT app"
  * Modifiez le message en spécifiant uniquement les trois ingrédients sans espace : Value1 Value2 Value3
  * Sauvegarder votre Applet IFTTT
  
  
### Ajout du périphérique
Cliquez sur "Configuration" / "Ajouter ou supprimer un périphérique" / "Store eedomus" / "Notifications IFTTT" / "Créer"  

  
*Voici les différents champs à renseigner:*

* [Obligatoire] - L'usage (Telegram, Twitter, Notifications..). Cette valeur ne sert que pour le nommage de votre capteur
* [Obligatoire] - Le code Key du service Webhooks IFTTT
* [Obligatoire] - Le nom de l'Event Webhooks IFTTT (Telegram_eedomus, Twitter_eedomus, IFTTT_eedomus..)

  
  
### Utilisation
Prédéfinissez des notifications dans les valeurs du périphérique créé par le plugin.  
Respectez bien la forme des valeurs et l'url du script appelé, à l'instar des valeurs par défaut fournies à la création.  
*NB1 : Ne supprimez pas la valeur cachée 9999 - [CHATBOT], qui permet le lien avec le plugin du même nom.*  
*NB2 : Ne supprimez pas la valeur cachée 99999 - [ASK], qui permet le lien avec le plugin du même nom.*  
  
Vous pouvez intégrer la valeur d'un ou plusieurs périphériques existants via son code API entre crochet, exemple : [123456].  
Vous pouvez sauter une ligne dans le message en utilisant [BR].  
Insérer la date [DATE] ou l'heure [TIME].  
Mettre en gras entre les balises [B] et [/B].  
Mettre en italique entre les balises [I] et [/I].  
  
![STEP1](https://i.imgur.com/S4GKzIJ.png)  
  
Lancez ensuite vos notifications depuis vos règles.  
NB : Les caractères spéciaux sont remplacés automatiquement, et le caractère ° est remplacé par ' (incompatibilité avec IFTTT...)  
  
![STEP2](https://i.imgur.com/HD1DoXS.png) 
  
  

Influman 2018  
therealinfluman@gmail.com  
[Paypal Me](https://www.paypal.me/influman "paypal.me")  
  

