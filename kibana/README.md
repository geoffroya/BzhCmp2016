# Kibana

Kibana 4 n'est pas fourni sous forme de paquet. Si on souhaite lancer plusieurs Kibana sur le m�me serveur avec des param�tre diff�rents, il faut faire un peu de travail soit-m�me.

C'est ce qui est fait ici :
- etc/init.d/kibana-appx : Init script pour une instance Kibana App-X
- etc/kibana/kibana-appx.yml : Fichier de configuration pour une instance Kibana App-X
- etc/logrotate.d/kibana : Configuration Logrotate

