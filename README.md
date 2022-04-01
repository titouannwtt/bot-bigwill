<div id="top"></div>

[![LinkedIn][linkedin-shield]][linkedin-url]

## Qu'est-ce que Bot-BigWill ?

BigWill est une stratégie de trading de crypto-monnaie créée par [CryptoRobots](https://github.com/CryptoRobotFr/) 
Ce bot est basé sur cette stratégie et va devoir être executé une fois par heure.

Il utilise l'API de la plateforme d'exchange [FTX](https://ftx.com/eu/referrals#a=102285520) pour intéragir avec le marché des cryptos-monnaies.
Le bot va détecter et choisir : quand acheter et quand vendre telle ou telle crypto-monnaie selon la stratégie BigWill (d'autres stratégies sont proposées sur le compte de [CryptoRobots](https://github.com/CryptoRobotFr/) .
/!\ Attention, je ne garantie en aucun cas les performances de ce bot, à utiliser à vos risques.

Depuis le fichier de configuration, il est possible de lister toutes les crypto-monnaies que l'on souhaite acheter et vendre.

Une fois le bot mis en place, vous devrez mettre un montant de départ sur la plateforme [FTX](https://ftx.com/eu/referrals#a=102285520), configurer vos API, paramétrer les notifications telegram puis laisser le bot faire son travail sur une longue période (1 mois, 1 an, 3 ans, 10 ans, ...) en espérant faire du profit.

## Code

Réalisé en Python, ce code a initialement été réalisé par :
[CryptoRobots](https://github.com/CryptoRobotFr/cBot-Project/blob/main/live_strategy/big_will_v2_live.py) 

J'ai rajouté du contenu à ce code permettant :
* de centraliser l'entièreté des configurations en un même fichier config.
* de recevoir des notifications lorsque le bot décide de vendre ou d'acheter une crypto-monnaie
* d'obtenir des statistiques détaillées sur l'évolution du solde du compte et un suivi des performances du bot sur du long terme (tout ceci est compris dans les notifications envoyées sur Telegram

### Installation

1. Héberger le bot de trading (tous les fichiers présents sur ce repos) sur une machine ubuntu ou debian continuellement allumée. Si vous rencontrez des difficultés, vous pouvez suivre [cette vidéo](https://www.youtube.com/watch?v=TbZ9BVAW_SA), le début de cette vidéo explique comment obtenir et se connecter à une machine ubuntu. 
2. Installer et configurer [telegram_send](https://github.com/rahiel/telegram-send#installation) sur votre machine pour recevoir les notifications Telegram. Si vous rencontrez des difficultés, vous pouvez suivre [cette vidéo](https://www.youtube.com/watch?v=dtLnO9AuFuk).
3. Entrez votre clé API de la plateforme [FTX](https://ftx.com/eu/referrals#a=102285520) dans le fichier de configuration.
4. Lancer le bot toutes les heures via la commande "python3 bot_bigwill.py" dans le crontab-e comme expliqué dans [la vidéo](https://www.youtube.com/watch?v=TbZ9BVAW_SA) de l'étape 1.

<p align="right">(<a href="#top">back to top</a>)</p>

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/titouan-wattelet-78a941162/