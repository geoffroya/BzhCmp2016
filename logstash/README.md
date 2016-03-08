# Logstash

La configuration est ici découpée en 3 parties :
- common : patterns grok, paramètres default (pour la JVM), logrotate
- buffer : configuration au niveau tampon. Ce logstash reçoit les logs et doit les pousser dans un tampon (j'ai choisi Redis, mais ça pourrait aussi bien être du Kafka)
- indexer : configuration de l'indexation : Récupération des logs dans le/les tampons, analyse en fonction de la méta-données **meta_fmt** (format) et indexation dans ES.
