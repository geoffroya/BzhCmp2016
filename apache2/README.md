# Apache

Apache est utilis� ici comme frontal pour N instances Kibana, via l'utilisation de virtual hosts :
- http://app1.mon-serveur-kibana.org
- http://app2.mon-serveur-kibana.org

Le configuration d�montre :
- La mise en place d'authentification et autorisation par groupe
- La coupure des op�rations de modification des settings Kibana, �vitant qu'un utilisateur d'un domaine A fasse pointer son kibana vers un domaine B
