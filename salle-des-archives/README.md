# Détection d'intrus

Juste après votre arrivée au bureau, vous venez dans votre messagerie l'email suivant de votre manager marqué ***URGENT***.
Vous avez 10 min pour le traiter et résoudre le problème.

# ![img](/assets/undercover.png)

## <u>Email</u>

Bonjour,

Nous avons régulièrement des attaques sur notre réseau informatique. Mais aujourd'hui, nous savous qu'un espion a eu accès à un de nos sites. Nous avons besoin de votre aide. Nous avons récuperer les informations sur les trames pour chacun des 4 sites. Pourriez vous nous dire sur quel site se trouve l'espion ?

Notre équipe IT vous a exporté un fichier d'historique de connexion provenant de notre IDS (Intrusion Dectection System). Nos sites ouvrent dans 10 minutes, une nouvelle intrusion de l'espion pourrait nous couter cher.

La situation étant sensible, les sites sont référencés par leurs noms de code: Alpha, Bravo, Charlie, Delta

Il vous faudra ensuite saisir dans l'interface le nom du site considéré

Merci d'avance de votre discrétion

Bonne chance on compte sur vous...

![image-20200824161301556](/assets/image-20200824161301556.png)

## OBJECTIF DE LA MISSION : LOCALISER LE SITE INFECTE

### Fichiers

Historique de log: [données analysée](https://github.com/vperrinfr/network_intrusion/blob/master/data/Train_data.csv)

Les trames des différents sites à évaluer: 

- **Alpha** : 0,"tcp","http","SF",233,2239,0,0,0,0,0,1,0,0,0,0,0,0,0,0,0,0,3,3,0,0,0,0,1,0,0,255,197,0.77,0.02,0,0,0,0,0,0

- **Bravo** : 31,"tcp","telnet","SF",197,1608,0,0,0,1,0,1,1,0,0,1,2,1,0,0,0,0,1,1,0,0,0,0,1,0,0,248,32,0.13,0.03,0,0,0,0,0,0

- **Charlie** : 0,"tcp","systat","S0",0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,239,20,1,1,0,0,0.08,0.07,0,255,20,0.08,0.08,0,0,1,1,0,0

- **Delta** : 0,"tcp","http","SF",277,4968,0,0,0,0,0,1,0,0,0,0,0,0,0,0,0,0,13,13,0,0,0,0,1,0,0,13,255,1,0,0.08,0.01,0,0,0,0

## Pour commencer

Aller dans l'interface Watson Studio, les données ont été uploadés dans le projet **Network_Intrusion_XX**

[Indice 1](https://github.com/vperrinfr/network_intrusion/blob/master/indice1.md)

[Indice 2](https://github.com/vperrinfr/network_intrusion/blob/master/indice2.md)


