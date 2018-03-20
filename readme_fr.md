# Installation
Gestion des Notifications via IFTTT pour Telegram, Twitter, Notifications, etc.
    
### Pr�requis en fonction de la notification souhait�e
  
R�cup�rer le code Key du service Webhooks de IFTTT.  
Dans IFTTT.com, apr�s avoir cr�� un compte le cas �ch�ant, recherchez (rubrique Search) le service Webhooks, et r�cup�rez votre code personnel KEY dans la rubrique Documentation.  
  
 ![WH](https://i.imgur.com/AsmQ2yR.png) 
  
Pour Telegram,  
  
  * Installez sur votre smartphone l'application Telegram, et �ventuellement l'application IFTTT (plus simple cependant de g�rer IFTTT.com depuis un �cran laptop)
  * Dans IFTTT, cherchez cette fois le service Telegram et appareillez le avec IFTTT. La proc�dure a pour finalit� de cr�er le Bot IFTTT sous Telegram.
  
 ![TLGM1](https://i.imgur.com/rTcoPX8.jpg) 

  * Retour dans IFTTT.com, cr�ez un nouvel Applet dans la rubrique My Applets (Bouton NEW APPLET)
  * Pour la partie +THIS, cherchez Webhooks, s�lectionnez "Receive a Web Request", et nommez le d�clencheur (Trigger) par exemple "Telegram_eedomus"
   
 ![WH2](https://i.imgur.com/Vjlfr91.png) 
  
  * Pour la partie +THAT, cherchez Telegram, s�lectionnez "Send Message", et modifiez Message Text en alignant les trois ingr�dients sans espace : Value1 Value2 Value3
  * Sauvegarder votre Applet IFTTT
 
 ![WH3](https://i.imgur.com/qUKzL96.png)  
  
  
Pour Twitter,  
  
Dans IFTTT, cherchez le service Twitter et appareillez le avec IFTTT, deux possibilit�s :   
- Soit vous avez pr�alablement cr�� un compte Twitter priv� compl�mentaire d�di� aux tweets de votre maison, et auquel vous abonnerez votre compte Twitter normal.
- Soit vous utilisez votre compte Twitter actuel et vous souhaiter un recevoir un message direct priv� (DM).  
  
  * Cr�ez un nouvel Applet dans la rubrique My Applets (Bouton NEW APPLET)
  * Pour la partie +THIS, cherchez Webhooks, s�lectionnez "Receive a Web Request", et nommez le d�clencheur (Trigger) par exemple "Twitter_eedomus"
  * Pour la partie +THAT, cherchez Twitter, s�lectionnez "Post a tweet" dans le 1er cas, ou "Send a direct message to yourself" dans le 2nd
  * Modifiez le message en sp�cifiant uniquement les trois ingr�dients sans espace : Value1 Value2 Value3
  * Sauvegarder votre Applet IFTTT
  
Pour Notifications IFTTT,
  
Ce service IFTTT r�alise un push notification direct (iOS ou Android).   
Il vous faut seulement installer l'application IFTTT sur votre smartphone.  
  
  * Cr�ez un nouvel Applet dans la rubrique My Applets (Bouton NEW APPLET)
  * Pour la partie +THIS, cherchez Webhooks, s�lectionnez "Receive a Web Request", et nommez le d�clencheur (Trigger) par exemple "IFTTT_eedomus"
  * Pour la partie +THAT, cherchez Notifications, s�lectionnez "Send a notification from the IFTTT app"
  * Modifiez le message en sp�cifiant uniquement les trois ingr�dients sans espace : Value1 Value2 Value3
  * Sauvegarder votre Applet IFTTT
  
  
### Ajout du p�riph�rique
Cliquez sur "Configuration" / "Ajouter ou supprimer un p�riph�rique" / "Store eedomus" / "Notifications IFTTT" / "Cr�er"  

  
*Voici les diff�rents champs � renseigner:*

* [Obligatoire] - L'usage (Telegram, Twitter, Notifications..). Cette valeur ne sert que pour le nommage de votre capteur
* [Obligatoire] - Le code Key du service Webhooks IFTTT
* [Obligatoire] - Le nom de l'Event Webhooks IFTTT (Telegram_eedomus, Twitter_eedomus, IFTTT_eedomus..)

  
  
### Utilisation
Pr�d�finissez des notifications dans les valeurs du p�riph�rique cr�� par le plugin.  
Respectez bien la forme des valeurs et l'url du script appel�, � l'instar des valeurs par d�faut fournies � la cr�ation.  
*NB1 : Ne supprimez pas la valeur cach�e 9999 - [CHATBOT], qui permet le lien avec le plugin du m�me nom.*  
*NB2 : Ne supprimez pas la valeur cach�e 99999 - [ASK], qui permet le lien avec le plugin du m�me nom.*  
  
Vous pouvez int�grer la valeur d'un ou plusieurs p�riph�riques existants via son code API entre crochet, exemple : [123456].  
Vous pouvez sauter une ligne dans le message en utilisant [BR].  
Ins�rer la date [DATE] ou l'heure [TIME].  
Mettre en gras entre les balises [B] et [/B].  
Mettre en italique entre les balises [I] et [/I].  
  
![STEP1](https://i.imgur.com/S4GKzIJ.png)  
  
Lancez ensuite vos notifications depuis vos r�gles.  
NB : Les caract�res sp�ciaux sont remplac�s automatiquement, et le caract�re � est remplac� par ' (incompatibilit� avec IFTTT...)  
  
![STEP2](https://i.imgur.com/HD1DoXS.png) 
  
  

Influman 2018  
therealinfluman@gmail.com  
[Paypal Me](https://www.paypal.me/influman "paypal.me")  
  

