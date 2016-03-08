# BzhCmp2016

Ce repo stocke les sources utilisées lors du talk "ELK en conditions réelles" du BrezihCamp 2016.

La vidéo du talk sera disponible prochainement.

Le but de ce talk est de présenter une décomposition des différents rôles pour mettre en place une collecte de logs au sein d'un SI "réel", en accord avec tous les interlocuteurs d'une DSI.

## Outils mis en oeuvre

Les outils mis en oeuvre sont :
- ELK
- Apache
- RSyslog
- Nxlog
- Redis

## Cible

La cible est une utilisation d'ES en multi-tenant :
- Un index distinct par domaine
- Un kibana distinct pour séparer les utilisateurs

La gestion du multi-tenant est dynamique, et gérée de manière transparente pour la chaîne de traitement, via l'utilisation de méta-données définies au niveau de la collecte.

L'intérêt du multi-tenant est de pouvoir se serveir d'ES pour avoir des comportements différents en fonction du domaine :
- Réplication ou non en fonction du domaine
- Paramètres de sharding différents en fonction du domaine
- Template différent
- Choix des noeuds ES en fonction du domaine
- ...


