# Logstash

La configuration est ici d�coup�e en 3 parties :
- common : patterns grok, param�tres default (pour la JVM), logrotate
- buffer : configuration au niveau tampon. Ce logstash re�oit les logs et doit les pousser dans un tampon (j'ai choisi Redis, mais �a pourrait aussi bien �tre du Kafka)
- indexer : configuration de l'indexation : R�cup�ration des logs dans le/les tampons, analyse en fonction de la m�ta-donn�es **meta_fmt** (format) et indexation dans ES.
