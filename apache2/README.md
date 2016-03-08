# Apache

Apache est utilisé ici comme frontal pour N instances Kibana, via l'utilisation de virtual hosts :
- http://app1.mon-serveur-kibana.org
- http://app2.mon-serveur-kibana.org

Le configuration démontre :
- La mise en place d'authentification et autorisation par groupe
- La coupure des opérations de modification des settings Kibana, évitant qu'un utilisateur d'un domaine A fasse pointer son kibana vers un domaine B
